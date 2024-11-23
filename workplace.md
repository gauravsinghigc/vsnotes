# system update @ 21 November 2024

@security updates for system including login and athentications.

- hash('sha256', random_bytes(32)) for form submission and validations modified
- // Save session with secure params
session_set_cookie_params([
    'lifetime' => 0, // Session cookie lasts only as long as the browser is open
    'path' => '/',
    'domain' => DOMAIN, // Use the constant DOMAIN
    'secure' => true, // Only send cookie over HTTPS
    'httponly' => true, // Prevent JavaScript access to the cookie
    'samesite' => 'Strict', // Prevent cross-site requests
]);

//session_start()
session_start();

- //set login user in cookie
            setcookie(
                'APP_LOGIN_USER_ID', // Cookie name
                $UserId,         // Cookie value
                time() + 86400,  // Expiry time (24 hours = 86400 seconds)
                '/',             // Path (accessible site-wide)
                DOMAIN,          // Domain (constant used here)
                true,            // Secure (only over HTTPS)
                true             // HttpOnly (not accessible via JavaScript)
            );
- if (isset($_COOKIE['APP_LOGIN_USER_ID'])) {
    $LoginUserId = $_COOKIE['APP_LOGIN_USER_ID'];

    //store cookie value in session
    $_SESSION['APP_LOGIN_USER_ID'] = $LoginUserId;

    //session check
    if (isset($_SESSION['APP_LOGIN_USER_ID']) != null) {
        $UserId = $_SESSION['APP_LOGIN_USER_ID'];

        //user constants
        define("LOGIN_USER_ID", $UserId);
        define("LOGIN_UserId", FETCH("SELECT UserId FROM users where UserId='$UserId'", "UserId"));
        define("LOGIN_UserFullName", FETCH("SELECT UserFullName FROM users where UserId='$UserId'", "UserFullName"));
        define("LOGIN_UserPhoneNumber", FETCH("SELECT UserPhoneNumber FROM users where UserId='$UserId'", "UserPhoneNumber"));
        define("LOGIN_UserEmailId", FETCH("SELECT UserEmailId from users where UserId='$UserId'", "UserEmailId"));
        define("LOGIN_UserCreatedAt", FETCH("SELECT UserCreatedAt FROM users where UserId='$UserId'", "UserCreatedAt"));
        define("LOGIN_UserUpdatedAt", FETCH("SELECT UserUpdatedAt FROM users where UserId='$UserId'", "UserUpdatedAt"));
        define("LOGIN_UserStatus", FETCH("SELECT UserStatus FROM users where UserId='$UserId'", "UserStatus"));
        define("LOGIN_UserProfileImage1", FETCH("SELECT UserProfileImage FROM users WHERE UserId='$UserId'", "UserProfileImage"));
        define("LOGIN_UserType", FETCH("SELECT UserType FROM users WHERE UserId='$UserId'", "UserType"));

        //user image
        if (LOGIN_UserProfileImage1 == "default.png") {
            define("LOGIN_UserProfileImage", STORAGE_URL_D . "/default.png");
        } else {
            define("LOGIN_UserProfileImage", STORAGE_URL_U . "/" . LOGIN_UserId . "/img/" . LOGIN_UserProfileImage1);
        }

        //no login
    } else {
        header("location:" . DOMAIN . "/auth/");
    }

    //no login
} else {
    header("location:" . DOMAIN . "/auth/");
}
- 
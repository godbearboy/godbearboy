<head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=no, viewport-fit=cover">
    <title>Hello World</title>
    <link rel="shortcut icon" href="./assets/image/favicon.ico">
    <link rel="apple-touch-icon" sizes="57x57" href="./assets/image/apple-icon-57x57.png">
    <link rel="apple-touch-icon" sizes="60x60" href="./assets/image/apple-icon-60x60.png">
    <link rel="apple-touch-icon" sizes="72x72" href="./assets/image/apple-icon-72x72.png">
    <link rel="apple-touch-icon" sizes="76x76" href="./assets/image/apple-icon-76x76.png">
    <link rel="apple-touch-icon" sizes="114x114" href="./assets/image/apple-icon-114x114.png">
    <link rel="apple-touch-icon" sizes="120x120" href="./assets/image/apple-icon-120x120.png">
    <link rel="apple-touch-icon" sizes="144x144" href="./assets/image/apple-icon-144x144.png">
    <link rel="apple-touch-icon" sizes="152x152" href="./assets/image/apple-icon-152x152.png">
    <link rel="apple-touch-icon" sizes="180x180" href="./assets/image/apple-icon-180x180.png">
    <link rel="icon" type="image/png" sizes="192x192" href="./assets/image/android-icon-192x192.png">
    <link rel="icon" type="image/png" sizes="32x32" href="./assets/image/favicon-32x32.png">
    <link rel="icon" type="image/png" sizes="96x96" href="./assets/image/favicon-96x96.png">
    <link rel="icon" type="image/png" sizes="16x16" href="./assets/image/favicon-16x16.png">
    <link rel="manifest" href="./manifest.json">
    <meta name="msapplication-TileColor" content="#ffffff">
    <meta name="msapplication-TileImage" content="/ms-icon-144x144.png">
    <meta name="theme-color" content="#ffffff">
    <!-- LIFF -->
    <script src="https://static.line-scdn.net/liff/edge/2.1/sdk.js"></script>
    <!-- vConsole -->
    <script src="./assets/js/vconsole.min.js"></script>
    <script src="./assets/js/liff-starter-V2.min.js"></script>
    <!-- Bootstrap -->
    <link rel="stylesheet" href="./assets/css/bootstrap.min.css">
    <!-- Custom styles for this template -->
    <link href="./assets/css/floating-labels.css" rel="stylesheet">
</head>


<body data-gr-c-s-loaded="true">
    <form class="form-signin" id="content">
        <div class="text-center mb-4">
            <h1 class="h3 mb-3 font-weight-strong">Hello World</h1>
            <p align="center" style="font-size: 15px;" id="greet">Send a liff message with the set parameters</p>
        </div>
        <div class="form-label-group">
            <select class="custom-select d-block w-100" id="type" onchange="changeType()" required>
                <option value="choose" disable hidden selected>Choose Message Type</option>
                <option value="profile">Profile</option>
                <option value="text">Text</option>
                <option value="image">Image</option>
                <option value="video">Video</option>
                <option value="audio">Audio</option>
                <option value="sticker">Sticker</option>
                <option value="stickerimage">Sticker Image</option>
                <option value="messages">Messages</option>
                <option value="messagesUrl">Messages Url</option>
                <option value="scanQr">Scan QR Code</option>
                <option value="liffToken">Get Liff Token</option>
                <option value="genToken">Generate LINE Token</option>
            </select>
        </div>
        <div class="form-label-group">
            <div class="custom-control custom-checkbox">
                <input type="checkbox" id="share" class="custom-control-input">
                <label for="share" class="custom-control-label">Share Message?</label>
            </div>
        </div>
        <a href="#" id="liffSendMessage" class="btn btn-lg btn-primary btn-block">Send Liff Message</a>
        <p class="mt-5 mb-3 text-muted text-center">© 2019 Hello World</p>
    </form>
</body>

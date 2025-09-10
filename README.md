<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Gajindu Yashmika | Full Stack Developer</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        /* Base Styles */
        body {
            font-family: 'Poppins', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f9;
            color: #333;
        }
        h1, h3 {
            margin: 0;
            color: #0e75b6;
        }
        p {
            font-size: 1rem;
            color: #555;
        }

        /* Layout and Centering */
        .container {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            text-align: center;
        }

        /* Profile Image Animation */
        .profile-img {
            border-radius: 50%;
            width: 150px;
            height: 150px;
            margin-bottom: 20px;
            transition: transform 0.3s ease;
        }
        .profile-img:hover {
            transform: scale(1.1);
        }

        /* Social Icons */
        .social-icons {
            margin: 20px 0;
        }
        .social-icons a {
            margin: 0 10px;
            text-decoration: none;
            color: #333;
            transition: transform 0.3s ease;
        }
        .social-icons a:hover {
            transform: scale(1.2);
            color: #0e75b6;
        }

        /* Button Styles */
        .btn {
            padding: 10px 20px;
            border: 2px solid #0e75b6;
            background-color: transparent;
            color: #0e75b6;
            font-weight: 600;
            text-decoration: none;
            border-radius: 5px;
            margin-top: 20px;
            transition: background-color 0.3s ease, color 0.3s ease;
        }
        .btn:hover {
            background-color: #0e75b6;
            color: white;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .container {
                padding: 20px;
            }
            .social-icons a {
                margin: 5px;
            }
        }

        /* Stats Animation */
        .stats {
            display: flex;
            justify-content: center;
            margin-top: 20px;
        }
        .stats img {
            margin: 0 15px;
        }
    </style>
</head>
<body>

    <div class="container">
        <!-- Profile Section -->
        <h1>Hi 👋, I'm Gajindu Yashmika</h1>
        <h3>A passionate Full Stack Developer from Sri Lanka</h3>

        <img class="profile-img" src="https://your-image-url.com" alt="Profile Image" />

        <!-- Profile Views Badge -->
        <p><img src="https://komarev.com/ghpvc/?username=yashmika5&label=Profile%20views&color=0e75b6&style=flat" alt="Profile views" /></p>

        <!-- Project Link Button -->
        <a class="btn" href="https://github.com/Yashmika5?tab=repositories" target="_blank">View My Projects</a>

        <p>📫 How to reach me: <strong>gajinduyashmika5@gmail.com</strong></p>

        <!-- Social Links -->
        <h3>Connect with me:</h3>
        <div class="social-icons">
            <a href="https://twitter.com/3" target="blank">
                <img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/twitter.svg" alt="Twitter" width="40" />
            </a>
            <a href="https://linkedin.com/in/yashmika5" target="blank">
                <img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="LinkedIn" width="40" />
            </a>
            <a href="https://kaggle.com/gajinduyashmika" target="blank">
                <img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/kaggle.svg" alt="Kaggle" width="40" />
            </a>
            <a href="https://fb.com/100081347803846" target="blank">
                <img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/facebook.svg" alt="Facebook" width="40" />
            </a>
            <a href="https://instagram.com/yashmika_5" target="blank">
                <img src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/instagram.svg" alt="Instagram" width="40" />
            </a>
        </div>

        <!-- Languages and Tools Section -->
        <h3>Languages and Tools:</h3>
        <div class="stats">
            <!-- Add images for tools -->
            <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="Python" width="40" />
            <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="JavaScript" width="40" />
            <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/react/react-original-wordmark.svg" alt="React" width="40" />
            <!-- Add more tool icons here -->
        </div>

        <!-- GitHub Stats -->
        <div class="stats">
            <img src="https://github-readme-stats.vercel.app/api/top-langs?username=yashmika5&show_icons=true&locale=en&layout=compact" alt="Top Languages" />
            <img src="https://github-readme-stats.vercel.app/api?username=yashmika5&show_icons=true&locale=en" alt="GitHub Stats" />
        </div>

        <!-- GitHub Streak -->
        <p><img align="center" src="https://github-readme-streak-stats.herokuapp.com/?user=yashmika5&" alt="GitHub Streak" /></p>
    </div>

</body>
</html>

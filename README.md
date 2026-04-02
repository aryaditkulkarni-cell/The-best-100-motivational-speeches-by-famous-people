<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>100 Best Motivational Speeches</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            background-color: #111;
            color: white;
        }

        header {
            background: #ff9800;
            padding: 15px;
            text-align: center;
            font-size: 24px;
            font-weight: bold;
        }

        .container {
            padding: 20px;
        }

        .speech {
            background: #222;
            margin: 15px 0;
            padding: 15px;
            border-radius: 10px;
        }

        .speech h3 {
            color: #ff9800;
        }

        button {
            padding: 10px;
            background: #ff9800;
            border: none;
            cursor: pointer;
            border-radius: 5px;
        }

        iframe {
            width: 100%;
            height: 200px;
            border-radius: 10px;
        }
    </style>
</head>

<body>

<header>
    💪 100 Best Motivational Speeches
</header>

<div class="container" id="speechList">
    <!-- Speeches will appear here -->
</div>

<script>
    const speeches = [
        {
            title: "Steve Jobs - Stay Hungry Stay Foolish",
            speaker: "Steve Jobs",
            video: "https://www.youtube.com/embed/UF8uR6Z6KLc"
        },
        {
            title: "Arnold Schwarzenegger - No Excuses",
            speaker: "Arnold Schwarzenegger",
            video: "https://www.youtube.com/embed/wnHW6o8WMas"
        },
        {
            title: "Denzel Washington - Fall Forward",
            speaker: "Denzel Washington",
            video: "https://www.youtube.com/embed/tbnzAVRZ9Xc"
        }
    ];

    const container = document.getElementById("speechList");

    speeches.forEach(s => {
        const div = document.createElement("div");
        div.className = "speech";

        div.innerHTML = `
            <h3>${s.title}</h3>
            <p>Speaker: ${s.speaker}</p>
            <iframe src="${s.video}" allowfullscreen></iframe>
        `;

        container.appendChild(div);
    });
</script>

</body>
</html>

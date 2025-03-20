# Studycafe.02
hello this is the update html for my new assignment projects. 
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Personal Website - Dong-A University</title>
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Arial', sans-serif; }
        body { background-color: #f0f0f5; color: #333; line-height: 1.6; }
        .main-container { display: flex; min-height: 100vh; }
        .panel { flex: 1; display: flex; flex-direction: column; justify-content: center; align-items: center; padding: 40px; text-align: center; transition: all 0.3s ease; }
        .panel:hover { flex: 1.5; }
        .black-panel { background-color: #222; color: white; }
        .blue-panel { background-color: #0085ca; color: white; }
        .white-panel { background-color: white; color: #222; }
        .btn { padding: 12px 25px; border: 2px solid currentColor; border-radius: 5px; text-decoration: none; font-weight: bold; transition: all 0.3s; display: inline-block; border-width: 3px; }
        .btn:hover { background-color: white; color: #222; }
        .black-outline { border-color: black; color: black; }
        .bio-container { display: none; position: fixed; top: 50%; left: 50%; transform: translate(-50%, -50%); background: white; padding: 30px; border-radius: 10px; text-align: center; box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.3); z-index: 1000; width: 80%; max-width: 350px; border: 3px solid #0085ca; }
        .close-btn { position: absolute; top: 10px; right: 15px; font-size: 1.5rem; cursor: pointer; color: #333; }
    </style>
</head>
<body>
    <div class="main-container">
        <div class="panel black-panel">
            <h2>Bio</h2>
            <p>Learn more about me, my academic journey, and research interests.</p>
            <button class="btn" onclick="openBio()">View Bio</button>
        </div>
        <div class="panel blue-panel">
            <h2>Assignments</h2>
            <p>Access my assignments and projects.</p>
            <a href="https://drive.google.com/drive/folders/1HEdPj6teJZ1kTmk-r2uzcGFjHI3ncf54" class="btn black-outline" target="_blank">Open Assignments</a>
        </div>
        <div class="panel white-panel">
            <h2>Meet Me!</h2>
            <p>Schedule a meeting by filling out my form.</p>
            <a href="https://forms.gle/7DCt8EuLRgdPb9p5A" class="btn black-outline" target="_blank">Book Appointment</a>
        </div>
    </div>
    
    <div id="bioSection" class="bio-container">
        <span class="close-btn" onclick="closeBio()">&times;</span>
        <h2>About Me</h2>
        <p><strong>Name:</strong> ALAM AL KAHAF</p>
        <p><strong>Phone:</strong> 010-9672-4615</p>
    </div>
    
    <script>
        function openBio() { 
            document.getElementById('bioSection').style.display = 'block';
        }
        function closeBio() { 
            document.getElementById('bioSection').style.display = 'none';
        }
    </script>
</body>
</html>

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Single Photo Upload</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            margin: 0;
            padding: 20px;
        }
        .container {
            max-width: 600px;
            margin: 0 auto;
        }
        .upload-section {
            background-color: white;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            text-align: center;
            margin-bottom: 30px;
        }
        h1 {
            color: #333;
            margin-bottom: 20px;
        }
        input[type="file"] {
            margin: 20px 0;
            padding: 10px;
            border: 2px dashed #ccc;
            border-radius: 5px;
            width: 100%;
            box-sizing: border-box;
        }
        button {
            background-color: #4CAF50;
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
        }
        button:hover {
            background-color: #45a049;
        }
        .photo-box {
            background-color: white;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            text-align: center;
            padding: 20px;
        }
        .photo-box img {
            max-width: 100%;
            max-height: 300px;
            object-fit: cover;
            border-radius: 5px;
        }
        .photo-box p {
            padding: 10px;
            margin: 0;
            font-size: 14px;
            color: #666;
        }
        .no-photo {
            color: #999;
            font-style: italic;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="upload-section">
            <h1>Upload Your Photo</h1>
            <form id="uploadForm" enctype="multipart/form-data">
                <input type="file" id="photoInput" accept="image/*" required>
                <br>
                <button type="submit">Upload Photo</button>
            </form>
        </div>

        <h2>Uploaded Photo</h2>
        <div class="photo-box" id="photoBox">
            <p class="no-photo">No photo uploaded yet.</p>
        </div>
    </div>

    <script>
        // Load the single photo from localStorage on page load
        function loadPhoto() {
            const photoBox = document.getElementById('photoBox');
            const photoData = JSON.parse(localStorage.getItem('singlePhoto') || 'null');
            if (photoData) {
                photoBox.innerHTML = `
                    <img src="${photoData.src}" alt="Uploaded Photo">
                    <p>Uploaded on ${photoData.timestamp}</p>
                `;
            } else {
                photoBox.innerHTML = '<p class="no-photo">No photo uploaded yet.</p>';
            }
        }

        // Handle form submission (replaces any existing photo)
        document.getElementById('uploadForm').addEventListener('submit', function(event) {
            event.preventDefault();
            const fileInput = document.getElementById('photoInput');
            const file = fileInput.files[0];
            if (file) {
                const reader = new FileReader();
                reader.onload = function(e) {
                    const photoData = {
                        src: e.target.result,
                        timestamp: new Date().toLocaleString()
                    };
                    // Store only one photo (replaces previous)
                    localStorage.setItem('singlePhoto', JSON.stringify(photoData));
                    loadPhoto(); // Refresh display
                    fileInput.value = ''; // Reset input
                    alert('Photo uploaded! (Previous photo replaced if any.)');
                };
                reader.readAsDataURL(file);
            }
        });

        // Load photo on page load
        loadPhoto();
    </script>
</body>
</html>

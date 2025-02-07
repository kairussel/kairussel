# Create an HTML file with a password-protected message

html_content = """<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>VIRUS, DO NOT OPEN</title>
    <script>
        function checkPassword() {
            var password = prompt("Enter the password:");
            if (password === "09142003") {
                document.getElementById("message").style.display = "block";
            } else {
                alert("Incorrect password!");
            }
        }
    </script>
</head>
<body onload="checkPassword()">
    <h1 style="display: none;" id="message">Kamusta ang buhay buhay Bri</h1>
</body>
</html>
"""

# Save the file
file_path = "/mnt/data/VIRUS_DO_NOT_OPEN.html"
with open(file_path, "w") as file:
    file.write(html_content)

file_path




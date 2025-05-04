<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Auto Analysis Redirect</title>
  <style>
    body { font-family: Arial, sans-serif; padding: 20px; }
    button { margin: 10px 0; padding: 10px 20px; font-size: 16px; }
  </style>
</head>
<body>

  <h2>Content Analysis Redirect Demo</h2>
  <p>Click a content type to simulate automatic redirection:</p>

  <button onclick="redirectTo('text')">Analyze Text</button><br>
  <button onclick="redirectTo('bias')">Check Media Bias</button><br>
  <button onclick="redirectTo('social')">Find Social Media Post</button><br>
  <button onclick="redirectTo('forensics')">Image Forensics</button><br>
  <button onclick="redirectTo('reverse-image')">Reverse Image Search</button><br>
  <button onclick="redirectTo('image-verify')">Image Verification Assistant</button><br>

  <script>
    function redirectTo(type) {
      const redirects = {
        text: "https://gptzero.me/",
        bias: "https://mediabiasfactcheck.com/",
        social: "https://whopostedwhat.com/",
        forensics: "https://fotoforensics.com/",
        "reverse-image": "https://tineye.com/",
        "image-verify": "https://mever.iti.gr/forensics/"
      };

      const url = redirects[type];
      if (url) {
        window.location.href = url;
      } else {
        alert("Unknown content type.");
      }
    }
  </script>

</body>
</html>

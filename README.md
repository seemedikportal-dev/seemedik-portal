<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <title>Menu Unduh - Seemedik Portal</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f4f6f9;
      padding: 30px;
    }

    .card {
      background: #fff;
      padding: 20px;
      border-radius: 10px;
      max-width: 900px;
      margin: auto;
      box-shadow: 0 2px 10px rgba(0,0,0,0.1);
    }

    h2 {
      margin-bottom: 20px;
    }

    .file-item {
      display: flex;
      justify-content: space-between;
      align-items: center;
      padding: 12px;
      border-bottom: 1px solid #eee;
    }

    .file-item:last-child {
      border-bottom: none;
    }

    .btn {
      padding: 8px 14px;
      border: none;
      border-radius: 6px;
      cursor: pointer;
      text-decoration: none;
      color: #fff;
      background: #2563eb;
    }

    .btn:hover {
      background: #1e40af;
    }

    iframe {
      width: 100%;
      height: 500px;
      margin-top: 20px;
      display: none;
      border-radius: 8px;
      border: 1px solid #ddd;
    }
  </style>
</head>
<body>

  <div class="card">
    <h2>Menu Unduh Berkas MCU</h2>

    <div class="file-item">
      <div>
        <strong>FERO DELTA ADITYAWAN</strong><br>
        <small>MCU - 4 Juni 1996</small>
      </div>
      <div>
        <button class="btn" onclick="previewPDF()">Preview</button>
        <a class="btn" href="pdf/PT_Hillcon_Jaya_Sakti_FERO_DELTA_ADITYAWAN.pdf" download>Unduh</a>
      </div>
    </div>

    <iframe id="pdfViewer"></iframe>
  </div>

  <script>
    function previewPDF() {
      const viewer = document.getElementById("pdfViewer");
      viewer.src = "pdf/PT_Hillcon_Jaya_Sakti_FERO_DELTA_ADITYAWAN.pdf";
      viewer.style.display = "block";
    }
  </script>

</body>
</html>

<!DOCTYPE html>
<html lang="th">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>ตารางนัดเที่ยว</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f4f4f4;
      padding: 20px;
      text-align: center;
    }
    table {
      width: 100%;
      border-collapse: collapse;
      margin-top: 20px;
      background: white;
      box-shadow: 0 0 8px rgba(0,0,0,0.1);
    }
    th, td {
      border: 1px solid #ddd;
      padding: 12px;
    }
    th {
      background: #4caf50;
      color: white;
    }
    input {
      width: 95%;
      padding: 5px;
      border: none;
      background-color: #f9f9f9;
    }
    input:focus {
      background-color: #fff;
      outline: none;
    }
  </style>
</head>
<body>
  <h1>📅 นัดเที่ยว 1 – 15 ก.ค. 2025</h1>
  <table>
    <tr>
      <th>วันที่</th>
      <th>วัน</th>
      <th>ว่างไหม?</th>
      <th>ชื่อ</th>
      <th>อยากไปที่ไหน</th>
    </tr>
    <script>
      const days = ["อังคาร", "พุธ", "พฤหัส", "ศุกร์", "เสาร์",
                    "อาทิตย์", "จันทร์", "อังคาร", "พุธ", "พฤหัส",
                    "ศุกร์", "เสาร์", "อาทิตย์", "จันทร์", "อังคาร"];
      for (let i = 1; i <= 15; i++) {
        document.write(`
          <tr>
            <td>${i} ก.ค.</td>
            <td>${days[i - 1]}</td>
            <td><input type="text" placeholder="ว่าง / ไม่ว่าง"></td>
            <td><input type="text" placeholder="ชื่อคุณ"></td>
            <td><input type="text" placeholder="สถานที่"></td>
          </tr>
        `);
      }
    </script>
  </table>
</body>
</html>

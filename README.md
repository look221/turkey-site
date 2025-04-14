<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>خدمات الحلول المتكاملة</title>
  <style>
    body {
      font-family: 'Cairo', sans-serif;
      background-color: #f4f4f4;
      padding: 20px;
      color: #333;
    }
    h1 {
      text-align: center;
      color: #4CAF50;
    }
    .menu {
      max-width: 600px;
      margin: 20px auto;
      background: white;
      padding: 20px;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
    }
    .menu-item {
      margin-bottom: 20px;
      border-bottom: 1px solid #eee;
      padding-bottom: 15px;
    }
    .menu-item:last-child {
      border-bottom: none;
    }
    label, select, button {
      display: block;
      margin-top: 10px;
    }
    select, button {
      padding: 8px;
      border-radius: 5px;
      border: 1px solid #ccc;
      width: 100%;
      max-width: 300px;
    }
    button {
      background-color: #4CAF50;
      color: white;
      border: none;
      cursor: pointer;
    }
    button:hover {
      background-color: #45a049;
    }
  </style>
</head>
<body>

  <h1>خدمات الحلول المتكاملة</h1>

  <div class="menu">
    <div class="menu-item">
      <span>استخراج إقامة سياحية</span>
      <label for="type1">نوع الطلب:</label>
      <select id="type1">
        <option value="جديد">جديد</option>
        <option value="تجديد">تجديد</option>
        <option value="استشارة فقط">استشارة فقط</option>
      </select>
      <button onclick="order('استخراج إقامة سياحية', 'type1')">اطلب الخدمة</button>
    </div>
    <div class="menu-item">
      <span>تأمين صحي للإقامة</span>
      <label for="type2">نوع الطلب:</label>
      <select id="type2">
        <option value="شامل">شامل</option>
        <option value="للمقيمين فقط">للمقيمين فقط</option>
      </select>
      <button onclick="order('تأمين صحي للإقامة', 'type2')">اطلب الخدمة</button>
    </div>
    <div class="menu-item">
      <span>الاستشارات الجامعية والقبول الجامعي</span>
      <label for="type3">نوع الطلب:</label>
      <select id="type3">
        <option value="بكالوريوس">بكالوريوس</option>
        <option value="ماجستير">ماجستير</option>
        <option value="دكتوراه">دكتوراه</option>
      </select>
      <button onclick="order('الاستشارات الجامعية والقبول الجامعي', 'type3')">اطلب الخدمة</button>
    </div>
    <div class="menu-item">
      <span>خدمة استخراج فيزا سياحية</span>
      <label for="type4">نوع الطلب:</label>
      <select id="type4">
        <option value="تركيا">تركيا</option>
        <option value="بالي">بالي</option>
        <option value="الإمارات">الإمارات</option>
        <option value="دولة أخرى">دولة أخرى</option>
      </select>
      <button onclick="order('خدمة استخراج فيزا سياحية', 'type4')">اطلب الخدمة</button>
    </div>
    <div class="menu-item">
      <span>خدمات النقل واستقبال المطار</span>
      <label for="type5">نوع الطلب:</label>
      <select id="type5">
        <option value="من المطار إلى الفندق">من المطار إلى الفندق</option>
        <option value="من الفندق إلى المطار">من الفندق إلى المطار</option>
        <option value="جولة سياحية خاصة">جولة سياحية خاصة</option>
      </select>
      <button onclick="order('خدمات النقل واستقبال المطار', 'type5')">اطلب الخدمة</button>
    </div>
  </div>

  <script>
    function order(serviceName, selectId) {
      const type = document.getElementById(selectId).value;
      const whatsappNumber = '905526058765';
      const message = `مرحباً، أرغب في طلب الخدمة التالية: ${serviceName}\nنوع الطلب: ${type}`;
      const url = `https://wa.me/${whatsappNumber}?text=${encodeURIComponent(message)}`;
      window.open(url, '_blank');
    }
  </script>

</body>
</html>

خدمات تركيا المتكامله

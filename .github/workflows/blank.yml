<!DOCTYPE html>
<html>
<head>
  <title>연락하기</title>
</head>
<body>

<h2>연락 페이지</h2>

<p id="phone">불러오는 중...</p>

<button id="callBtn">전화하기</button>

<script>
const id = new URLSearchParams(location.search).get("id");

fetch("/api/" + id)
  .then(res => res.json())
  .then(data => {
    document.getElementById("phone").innerText = data.phone;

    document.getElementById("callBtn").onclick = () => {
      window.location.href = "tel:" + data.phone;
    };
  });
</script>

</body>
</html>

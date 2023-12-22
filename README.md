<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <script src="https://aframe.io/releases/1.2.0/aframe.min.js"></script>
  <script src="https://raw.githack.com/AR-js-org/AR.js/master/aframe/build/aframe-ar-nft.js"></script>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <a-scene id="scene" embedded arjs>
      <!-- Фортеця -->
      <a-entity position="0 0 0">
        <!-- Тіло фортеці -->
        <a-cylinder src="https://terracot.ua/storage/app/uploads/public/600/996/99d/thumb_9730_1700_1600_0_0_auto.webp" height="4" radius="4" color="#c0c0c0"></a-cylinder>
<a-box src="https://terracot.ua/storage/app/uploads/public/600/996/99d/thumb_9730_1700_1600_0_0_auto.webp" position="0 1.5 -4" width="4" height="3" depth="4" color="gray"></a-box>
 <a-cylinder src="https://terracot.ua/storage/app/uploads/public/600/996/99d/thumb_9730_1700_1600_0_0_auto.webp" position="0 3 -4" radius="1" height="2" color="gray"></a-cylinder>
 <a-cone src="https://terracot.ua/storage/app/uploads/public/600/996/99d/thumb_9730_1700_1600_0_0_auto.webp" position="0 4.5 -4" radius-bottom="1.5" radius-top="0" height="1.5" color="gray"></a-cone>
   </a-entity>
        <!-- Прапор -->
<a-entity position="0 6 -4" animation="property: rotation; to: 0 360 0; loop: true; dur: 5000">
        <a-plane position="0 4.5 0" width="4" height="2" color="#ff0000" id="flag"></a-plane>
            <a-plane width="2" height="1" color="red" text="value: Thank You Mario But Our Princess Is in Another Castle"></a-plane>
 <a-text value="Thank You Mario But Our Princess Is in Another Castle" color="white" wrap-count="25"></a-text>
      </a-entity>
 </a-entity>
        <!-- Анімація флагштоку -->
        <a-entity position="0 0 -4" animation="property: rotation; to: -90 0 0; loop: false; dur: 3000"></a-entity>
      <!-- Анімація прапора -->
      <a-animation attribute="rotation" dur="3000" to="0 360 0" repeat="indefinite"></a-animation>
      <!-- Анімація підняття прапора -->
      <a-animation attribute="position" dur="2000" to="0 6 0" repeat="1" direction="alternate" easing="ease-in-out" begin="flagAnimation"></a-animation>
  </a-scene>
</body>
</html>

<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Trái Đất Vector - Ô nhiễm & Giải pháp Khắc phục</title>
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body {
      overflow: hidden;
      background: #0b0f1a;
      font-family: 'Segoe UI', system-ui, sans-serif;
      color: #fff;
    }
    #canvas-container {
      width: 100vw;
      height: 100vh;
      position: relative;
    }
    canvas { display: block; }

    #info-panel {
      position: absolute;
      top: 24px;
      left: 24px;
      width: 340px;
      background: rgba(11, 15, 26, 0.92);
      border: 1px solid rgba(255,255,255,0.08);
      border-radius: 18px;
      padding: 20px 22px;
      backdrop-filter: blur(20px);
      z-index: 10;
      box-shadow: 0 12px 40px rgba(0,0,0,0.45);
    }
    #info-panel h1 {
      font-size: 18px;
      font-weight: 600;
      margin-bottom: 8px;
      display: flex;
      align-items: center;
      gap: 8px;
    }
    #info-panel p {
      font-size: 13.5px;
      line-height: 1.55;
      color: rgba(255,255,255,0.78);
    }

    #legend {
      position: absolute;
      bottom: 24px;
      left: 24px;
      background: rgba(11, 15, 26, 0.92);
      border: 1px solid rgba(255,255,255,0.08);
      border-radius: 18px;
      padding: 16px 20px;
      backdrop-filter: blur(20px);
      z-index: 10;
      font-size: 13px;
      box-shadow: 0 12px 40px rgba(0,0,0,0.45);
      max-width: 360px;
    }
    #legend strong {
      display: block;
      margin-bottom: 10px;
      font-size: 13px;
    }
    .legend-item {
      display: flex;
      align-items: center;
      gap: 10px;
      margin: 6px 0;
      color: rgba(255,255,255,0.82);
    }
    .dot {
      width: 12px;
      height: 12px;
      border-radius: 50%;
      flex-shrink: 0;
    }
    .dot.red { background: #ff3b3b; box-shadow: 0 0 12px #ff3b3b; }
    .dot.orange { background: #ff9f1a; box-shadow: 0 0 12px #ff9f1a; }
    .dot.yellow { background: #ffd60a; box-shadow: 0 0 12px #ffd60a; }
    .dot.blue { background: #00b4d8; box-shadow: 0 0 12px #00b4d8; }
    .dot.green { background: #00e676; box-shadow: 0 0 12px #00e676; }

    .solution-note {
      margin-top: 12px;
      padding-top: 10px;
      border-top: 1px solid rgba(255,255,255,0.1);
      font-size: 12.5px;
      color: #00e676;
      line-height: 1.45;
    }

    #controls {
      position: absolute;
      top: 24px;
      right: 24px;
      display: flex;
      flex-direction: column;
      gap: 10px;
      z-index: 10;
    }
    button {
      background: rgba(11, 15, 26, 0.92);
      border: 1px solid rgba(255,255,255,0.1);
      color: #fff;
      padding: 11px 18px;
      border-radius: 12px;
      font-size: 13.5px;
      cursor: pointer;
      backdrop-filter: blur(20px);
      transition: all 0.2s;
    }
    button:hover {
      background: rgba(255, 59, 59, 0.9);
      border-color: #ff3b3b;
      transform: translateY(-1px);
    }

    #popup {
      position: absolute;
      display: none;
      background: rgba(11, 15, 26, 0.96);
      border-radius: 14px;
      padding: 16px 18px;
      max-width: 310px;
      z-index: 20;
      pointer-events: none;
      border: 1px solid;
      backdrop-filter: blur(16px);
      box-shadow: 0 12px 40px rgba(0,0,0,0.5);
    }
    #popup h3 {
      font-size: 15px;
      margin-bottom: 6px;
    }
    #popup p {
      font-size: 13px;
      line-height: 1.5;
      color: rgba(255,255,255,0.88);
    }
  </style>
</head>
<body>
  <div id="canvas-container">
    <div id="info-panel">
      <h1>🌍 Ô nhiễm & Giải pháp Khắc phục</h1>
      <p>Mô hình vector thể hiện các điểm nóng ô nhiễm và các giải pháp khắc phục bền vững. Click vào điểm sáng để xem chi tiết.</p>
    </div>

    <div id="legend">
      <strong>Chú thích</strong>
      <div class="legend-item"><div class="dot red"></div> Ô nhiễm nghiêm trọng</div>
      <div class="legend-item"><div class="dot orange"></div> Ô nhiễm cao</div>
      <div class="legend-item"><div class="dot yellow"></div> Ô nhiễm trung bình</div>
      <div class="legend-item"><div class="dot blue"></div> Hoàng Sa / Trường Sa</div>
      <div class="legend-item"><div class="dot green"></div> Giải pháp khắc phục</div>

      <div class="solution-note">
        <strong>Giải pháp khắc phục nổi bật:</strong><br>
        • Costa Rica – Phục hồi rừng<br>
        • Singapore – Quản lý nước thông minh<br>
        • Đan Mạch – Năng lượng gió<br>
        • Bhutan – Quốc gia carbon âm<br>
        • Cà Mau – Rừng ngập mặn<br>
        • Ninh Thuận – Điện gió
      </div>
    </div>

    <div id="controls">
      <button id="btn-rotate">Tạm dừng xoay</button>
      <button id="btn-reset">Đặt lại góc nhìn</button>
    </div>

    <div id="popup">
      <h3 id="popup-title"></h3>
      <p id="popup-desc"></p>
    </div>
  </div>

  <script src="https://cdnjs.cloudflare.com/ajax/libs/three.js/r128/three.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/three@0.128.0/examples/js/controls/OrbitControls.js"></script>

  <script>
    const container = document.getElementById('canvas-container');
    const scene = new THREE.Scene();
    scene.background = new THREE.Color(0x0b0f1a);

    // Sao nền
    const starsGeo = new THREE.BufferGeometry();
    const starCount = 3000;
    const starPos = new Float32Array(starCount * 3);
    for (let i = 0; i < starCount * 3; i++) starPos[i] = (Math.random() - 0.5) * 2000;
    starsGeo.setAttribute('position', new THREE.BufferAttribute(starPos, 3));
    scene.add(new THREE.Points(starsGeo, new THREE.PointsMaterial({
      color: 0xffffff, size: 1.35, transparent: true, opacity: 0.75
    })));

    const camera = new THREE.PerspectiveCamera(42, window.innerWidth / window.innerHeight, 0.1, 1000);
    camera.position.set(0.2, 0.28, 2.9);

    const renderer = new THREE.WebGLRenderer({ antialias: true });
    renderer.setSize(window.innerWidth, window.innerHeight);
    renderer.setPixelRatio(Math.min(window.devicePixelRatio, 2));
    renderer.toneMapping = THREE.ACESFilmicToneMapping;
    renderer.toneMappingExposure = 1.65;
    container.appendChild(renderer.domElement);

    const controls = new THREE.OrbitControls(camera, renderer.domElement);
    controls.enableDamping = true;
    controls.dampingFactor = 0.06;
    controls.minDistance = 1.75;
    controls.maxDistance = 6;
    controls.autoRotate = true;
    controls.autoRotateSpeed = 0.4;

    // Ánh sáng
    scene.add(new THREE.AmbientLight(0x4a5070, 1.0));
    const dirLight = new THREE.DirectionalLight(0xffffff, 2.4);
    dirLight.position.set(5, 3, 4);
    scene.add(dirLight);
    const fillLight = new THREE.DirectionalLight(0x88aaff, 0.6);
    fillLight.position.set(-4, 2, -3);
    scene.add(fillLight);

    // ===== TRÁI ĐẤT =====
    const textureLoader = new THREE.TextureLoader();
    const earthTexture = textureLoader.load('https://raw.githubusercontent.com/mrdoob/three.js/master/examples/textures/planets/earth_atmos_2048.jpg');

    const earth = new THREE.Mesh(
      new THREE.SphereGeometry(1, 96, 96),
      new THREE.MeshStandardMaterial({
        map: earthTexture,
        roughness: 0.85,
        metalness: 0.03,
        emissive: new THREE.Color(0x111122),
        emissiveIntensity: 0.32
      })
    );
    scene.add(earth);

    // Khí quyển
    const atmosphere = new THREE.Mesh(
      new THREE.SphereGeometry(1.075, 64, 64),
      new THREE.ShaderMaterial({
        vertexShader: `
          varying vec3 vNormal;
          void main() {
            vNormal = normalize(normalMatrix * normal);
            gl_Position = projectionMatrix * modelViewMatrix * vec4(position, 1.0);
          }
        `,
        fragmentShader: `
          varying vec3 vNormal;
          void main() {
            float intensity = pow(0.66 - dot(vNormal, vec3(0,0,1)), 2.1);
            gl_FragColor = vec4(0.28, 0.55, 1.0, 1.0) * intensity * 1.1;
          }
        `,
        blending: THREE.AdditiveBlending,
        side: THREE.BackSide,
        transparent: true
      })
    );
    scene.add(atmosphere);

    // ==================== DỮ LIỆU ====================
    const points = [
      { name: "New Delhi, Ấn Độ", lat: 28.61, lon: 77.21, type: "red", desc: "Ô nhiễm không khí cực nghiêm trọng (AQI > 300). Cần giảm đốt rơm rạ và cải thiện giao thông công cộng." },
      { name: "Bắc Kinh, Trung Quốc", lat: 39.90, lon: 116.40, type: "red", desc: "Ô nhiễm bụi mịn cao. Giải pháp: chuyển đổi năng lượng sạch, hạn chế phương tiện dầu." },
      { name: "Lahore, Pakistan", lat: 31.55, lon: 74.34, type: "red", desc: "Một trong những thành phố ô nhiễm nhất thế giới." },
      { name: "Jakarta, Indonesia", lat: -6.21, lon: 106.85, type: "orange", desc: "Ô nhiễm không khí và nước. Cần nâng cấp hệ thống xử lý nước thải." },
      { name: "TP. Hồ Chí Minh", lat: 10.82, lon: 106.63, type: "orange", desc: "Ô nhiễm không khí + kênh rạch. Giải pháp: phát triển xe điện và xử lý nước thải tập trung." },
      { name: "Hà Nội", lat: 21.03, lon: 105.85, type: "orange", desc: "Bụi mịn cao vào mùa đông. Cần kiểm soát khí thải công nghiệp và giao thông." },
      { name: "Sông Hằng", lat: 25.3, lon: 83.0, type: "red", desc: "Sông bị ô nhiễm nặng. Cần xử lý nước thải và nâng cao ý thức cộng đồng." },
      { name: "Amazon - Phá rừng", lat: -3.5, lon: -62.0, type: "orange", desc: "Mất rừng nghiêm trọng. Giải pháp: bảo tồn và phục hồi rừng quy mô lớn." },
      { name: "Biển Đông - Rác nhựa", lat: 12.5, lon: 114.5, type: "yellow", desc: "Điểm nóng rác thải nhựa. Cần giảm nhựa dùng một lần và thu gom đại dương." },

      { name: "Quần đảo Hoàng Sa", lat: 16.50, lon: 112.00, type: "blue", desc: "Thuộc chủ quyền Việt Nam. Cần bảo vệ hệ sinh thái biển, chống đánh bắt trái phép và rác thải nhựa." },
      { name: "Quần đảo Trường Sa", lat: 10.00, lon: 114.20, type: "blue", desc: "Thuộc chủ quyền Việt Nam. Ưu tiên bảo tồn rạn san hô và kiểm soát ô nhiễm biển." },

      { name: "Costa Rica - Phục hồi rừng", lat: 9.75, lon: -83.75, type: "green", desc: "Giải pháp thành công: Chi trả dịch vụ hệ sinh thái + du lịch bền vững → phục hồi hơn 50% diện tích rừng." },
      { name: "Singapore - Quản lý nước", lat: 1.35, lon: 103.82, type: "green", desc: "Giải pháp: Công nghệ NEWater + thu gom nước mưa + quản lý thông minh → tự chủ nguồn nước." },
      { name: "Đan Mạch - Năng lượng gió", lat: 56.26, lon: 9.50, type: "green", desc: "Giải pháp: Đầu tư mạnh điện gió → hướng tới 100% năng lượng tái tạo." },
      { name: "Bhutan - Carbon âm", lat: 27.50, lon: 90.50, type: "green", desc: "Giải pháp: Bảo vệ rừng (>70% diện tích) + thủy điện sạch → trở thành quốc gia carbon âm." },
      { name: "Cà Mau - Rừng ngập mặn", lat: 9.15, lon: 105.15, type: "green", desc: "Giải pháp Việt Nam: Trồng và phục hồi rừng ngập mặn → chống biến đổi khí hậu, bảo vệ bờ biển, tạo sinh kế." },
      { name: "Ninh Thuận - Điện gió", lat: 11.60, lon: 108.90, type: "green", desc: "Giải pháp Việt Nam: Phát triển điện gió quy mô lớn → giảm phát thải, chuyển đổi năng lượng sạch." }
    ];

    function latLonToVec3(lat, lon, r = 1.032) {
      const phi = (90 - lat) * Math.PI / 180;
      const theta = (lon + 180) * Math.PI / 180;
      return new THREE.Vector3(
        -r * Math.sin(phi) * Math.cos(theta),
         r * Math.cos(phi),
         r * Math.sin(phi) * Math.sin(theta)
      );
    }

    // Gắn marker vào Trái Đất
    const markerGroup = new THREE.Group();
    earth.add(markerGroup);

    const markers = [];
    points.forEach((p) => {
      let color, size;
      if (p.type === "red")        { color = 0xff3b3b; size = 0.039; }
      else if (p.type === "orange"){ color = 0xff9f1a; size = 0.034; }
      else if (p.type === "yellow"){ color = 0xffd60a; size = 0.030; }
      else if (p.type === "blue")  { color = 0x00b4d8; size = 0.037; }
      else                        { color = 0x00e676; size = 0.038; }

      const marker = new THREE.Mesh(
        new THREE.SphereGeometry(size, 32, 32),
        new THREE.MeshBasicMaterial({ color, transparent: true, opacity: 0.96 })
      );
      marker.position.copy(latLonToVec3(p.lat, p.lon));
      marker.userData = p;

      const ring = new THREE.Mesh(
        new THREE.RingGeometry(size * 1.55, size * 2.05, 64),
        new THREE.MeshBasicMaterial({ color, transparent: true, opacity: 0.55, side: THREE.DoubleSide })
      );
      ring.lookAt(0, 0, 0);
      marker.add(ring);

      const glow = new THREE.Mesh(
        new THREE.SphereGeometry(size * 2.6, 32, 32),
        new THREE.MeshBasicMaterial({ color, transparent: true, opacity: 0.16, side: THREE.BackSide })
      );
      marker.add(glow);

      markerGroup.add(marker);
      markers.push(marker);
    });

    // Tương tác
    const raycaster = new THREE.Raycaster();
    const mouse = new THREE.Vector2();
    const popup = document.getElementById('popup');
    const popupTitle = document.getElementById('popup-title');
    const popupDesc = document.getElementById('popup-desc');

    window.addEventListener('click', e => {
      mouse.x = (e.clientX / innerWidth) * 2 - 1;
      mouse.y = -(e.clientY / innerHeight) * 2 + 1;
      raycaster.setFromCamera(mouse, camera);
      const hits = raycaster.intersectObjects(markers);

      if (hits.length) {
        const d = hits[0].object.userData;
        popupTitle.textContent = d.name;
        popupDesc.textContent = d.desc;

        const colorMap = {
          red: "#ff3b3b",
          orange: "#ff9f1a",
          yellow: "#ffd60a",
          blue: "#00b4d8",
          green: "#00e676"
        };
        popup.style.borderColor = colorMap[d.type];
        popupTitle.style.color = colorMap[d.type];
        popup.style.display = 'block';
        popup.style.left = (e.clientX + 16) + 'px';
        popup.style.top = (e.clientY + 16) + 'px';
      } else {
        popup.style.display = 'none';
      }
    });

    // ===== NÚT ĐIỀU KHIỂN (đã sửa) =====
    let isRotating = true;

    document.getElementById('btn-rotate').onclick = () => {
      isRotating = !isRotating;
      controls.autoRotate = isRotating;
      document.getElementById('btn-rotate').textContent = isRotating ? 'Tạm dừng xoay' : 'Tiếp tục xoay';
    };

    document.getElementById('btn-reset').onclick = () => {
      camera.position.set(0.2, 0.28, 2.9);
      controls.target.set(0, 0, 0);
    };

    // Animation
    function animate() {
      requestAnimationFrame(animate);

      // Chỉ xoay Trái Đất khi isRotating = true
      if (isRotating) {
        earth.rotation.y += 0.00038;
        atmosphere.rotation.y += 0.00012;
      }

      // Hiệu ứng nhịp đập vẫn chạy
      const t = Date.now() * 0.002;
      markers.forEach((m, i) => {
        const s = 1 + Math.sin(t + i * 0.65) * 0.13;
        m.scale.setScalar(s);
      });

      controls.update();
      renderer.render(scene, camera);
    }
    animate();

    window.addEventListener('resize', () => {
      camera.aspect = innerWidth / innerHeight;
      camera.updateProjectionMatrix();
      renderer.setSize(innerWidth, innerHeight);
    });
  </script>
</body>
</html>

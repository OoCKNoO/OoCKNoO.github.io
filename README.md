# OoCKNoO
A showcase of my work.
<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Noina | 3D Portfolio</title>

    <!-- Three.js -->
    <script src="https://cdn.jsdelivr.net/npm/three@0.160.0/build/three.min.js"></script>

    <style>
        @import url('https://fonts.googleapis.com/css2?family=Itim&family=Kanit:wght@300;400;500;600&display=swap');

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            overflow: hidden;
            font-family: 'Kanit', sans-serif;
            background:
                radial-gradient(circle at top left, #ffe4ef, transparent 40%),
                radial-gradient(circle at bottom right, #dfe9ff, transparent 40%),
                #fff8f3;
            color: #725f67;
        }

        canvas {
            position: fixed;
            top: 0;
            left: 0;
            z-index: 0;
        }

        /* Main UI */

        .container {
            position: relative;
            z-index: 2;
            min-height: 100vh;
            pointer-events: none;
        }

        /* Navbar */

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 30px 7%;
        }

        .logo {
            font-family: 'Itim', cursive;
            font-size: 2rem;
            color: #e79ab5;
            letter-spacing: 1px;
        }

        .badge {
            background: rgba(255,255,255,0.65);
            backdrop-filter: blur(12px);
            padding: 8px 18px;
            border-radius: 30px;
            font-size: 0.85rem;
            box-shadow: 0 5px 20px rgba(200,150,170,0.15);
        }

        /* Hero */

        .hero {
            min-height: 78vh;
            display: flex;
            align-items: center;
            padding: 0 10%;
        }

        .content {
            max-width: 650px;
            animation: fadeUp 1.2s ease;
        }

        .hello {
            display: inline-block;

            background: #ffdce9;

            padding: 8px 20px;

            border-radius: 30px;

            margin-bottom: 20px;

            font-size: 1rem;

            color: #b76f8b;

            box-shadow: 0 8px 20px rgba(230,150,180,0.2);
        }

        h1 {
            font-family: 'Itim', cursive;

            font-size: clamp(3.5rem, 7vw, 7rem);

            font-weight: 400;

            line-height: 1;

            color: #c985a1;

            text-shadow:
                3px 3px 0 #fff,
                6px 6px 20px rgba(190,120,150,0.15);
        }

        .nickname {
            color: #8ba8d8;
        }

        .subtitle {
            margin-top: 25px;

            font-size: 1.3rem;

            line-height: 1.8;

            color: #786971;
        }

        /* Information Cards */

        .info-grid {

            display: grid;

            grid-template-columns: repeat(2, minmax(180px, 1fr));

            gap: 15px;

            margin-top: 35px;

            max-width: 600px;

        }

        .card {

            background: rgba(255,255,255,0.65);

            backdrop-filter: blur(15px);

            border: 1px solid rgba(255,255,255,0.8);

            padding: 18px 22px;

            border-radius: 22px;

            box-shadow:

                0 12px 35px rgba(150,120,140,0.12);

            transition: 0.3s;

        }

        .card:hover {

            transform: translateY(-5px);

        }

        .card span {

            font-size: 1.5rem;

            display: block;

            margin-bottom: 5px;

        }

        .card h3 {

            font-size: 0.85rem;

            font-weight: 400;

            color: #c58da4;

        }

        .card p {

            font-size: 1rem;

            margin-top: 3px;

        }

        /* Bottom Text */

        .footer {

            position: absolute;

            bottom: 25px;

            width: 100%;

            text-align: center;

            color: #aa9ca2;

            font-size: 0.85rem;

        }

        /* Floating decoration */

        .floating-text {

            position: absolute;

            right: 10%;

            top: 20%;

            background: rgba(255,255,255,0.55);

            backdrop-filter: blur(12px);

            padding: 15px 22px;

            border-radius: 25px;

            transform: rotate(5deg);

            box-shadow: 0 10px 30px rgba(160,130,150,0.12);

            font-family: 'Itim';

            font-size: 1.3rem;

            color: #9d8bc7;

        }

        /* Animation */

        @keyframes fadeUp {

            from {

                opacity: 0;

                transform: translateY(30px);

            }

            to {

                opacity: 1;

                transform: translateY(0);

            }

        }

        /* Mobile */

        @media (max-width: 768px) {

            nav {

                padding: 20px;

            }

            .hero {

                padding: 0 7%;

                align-items: flex-start;

                padding-top: 60px;

            }

            h1 {

                font-size: 4rem;

            }

            .subtitle {

                font-size: 1rem;

            }

            .info-grid {

                grid-template-columns: 1fr;

            }

            .floating-text {

                right: 5%;

                top: 13%;

                font-size: 1rem;

            }

        }

    </style>
</head>

<body>

    <div class="container">

        <nav>

            <div class="logo">
                Noina's Portfolio ✿
            </div>

            <div class="badge">
                🎮 Game & Animation
            </div>

        </nav>


        <main class="hero">

            <section class="content">

                <div class="hello">
                    🌷 Hello, Nice to meet you!
                </div>

                <h1>
                    จารุณี
                    <br>

                    <span class="nickname">
                        น้อยหน่า
                    </span>
                </h1>

                <p class="subtitle">

                    นักออกแบบเกมและแอนิเมชัน
                    <br>

                    ผู้หลงใหลในโลกของ
                    <b>Creativity, Games & Art</b> ✨

                </p>


                <div class="info-grid">

                    <div class="card">

                        <span>👩🏻‍🎓</span>

                        <h3>ชื่อ</h3>

                        <p>
                            จารุณี แก้วพินิจ
                        </p>

                    </div>


                    <div class="card">

                        <span>🍈</span>

                        <h3>ชื่อเล่น</h3>

                        <p>
                            น้อยหน่า
                        </p>

                    </div>


                    <div class="card">

                        <span>🎮</span>

                        <h3>สาขาวิชา</h3>

                        <p>
                            การออกแบบเกมและแอนิเมชัน
                        </p>

                    </div>


                    <div class="card">

                        <span>🏫</span>

                        <h3>สถานศึกษา</h3>

                        <p>
                            Rajamangala University
                            of Technology Rattanakosin
                        </p>

                    </div>

                </div>

            </section>

        </main>


        <div class="floating-text">
            ✨ Let's create something magical!
        </div>


        <div class="footer">
            Made with ☁️ Three.js & Creativity
        </div>

    </div>


    <script>

        /* =========================

           THREE.JS SETUP

        ========================= */

        const scene = new THREE.Scene();


        const camera = new THREE.PerspectiveCamera(

            60,

            window.innerWidth / window.innerHeight,

            0.1,

            100

        );


        camera.position.z = 8;


        const renderer = new THREE.WebGLRenderer({

            antialias: true,

            alpha: true

        });


        renderer.setSize(

            window.innerWidth,

            window.innerHeight

        );


        renderer.setPixelRatio(

            Math.min(window.devicePixelRatio, 2)

        );


        document.body.appendChild(

            renderer.domElement

        );


        /* =========================

           LIGHTING

        ========================= */

        const ambientLight = new THREE.AmbientLight(

            0xffffff,

            2

        );


        scene.add(

            ambientLight

        );


        const pointLight = new THREE.PointLight(

            0xffb6d2,

            3,

            30

        );


        pointLight.position.set(

            4,

            5,

            6

        );


        scene.add(

            pointLight

        );


        /* =========================

           PASTEL OBJECTS

        ========================= */

        const objects = [];


        const colors = [

            0xffb6cf,

            0xb9d8ff,

            0xcbb7f6,

            0xffd6a5,

            0xbde8d1

        ];


        function createObject() {

            const geometryType = Math.floor(

                Math.random() * 3

            );


            let geometry;


            if (geometryType === 0) {

                geometry = new THREE.SphereGeometry(

                    0.35,

                    32,

                    32

                );

            }

            else if (geometryType === 1) {

                geometry = new THREE.TorusGeometry(

                    0.3,

                    0.1,

                    16,

                    32

                );

            }

            else {

                geometry = new THREE.IcosahedronGeometry(

                    0.35,

                    1

                );

            }


            const material =

                new THREE.MeshStandardMaterial({

                    color:

                        colors[

                            Math.floor(

                                Math.random()

                                *

                                colors.length

                            )

                        ],

                    roughness: 0.4,

                    metalness: 0.05

                });


            const mesh = new THREE.Mesh(

                geometry,

                material

            );


            mesh.position.set(

                (Math.random() - 0.5) * 15,

                (Math.random() - 0.5) * 10,

                (Math.random() - 0.5) * 5

            );


            mesh.rotation.set(

                Math.random() * Math.PI,

                Math.random() * Math.PI,

                Math.random() * Math.PI

            );


            mesh.userData = {

                speed:

                    0.002

                    +

                    Math.random() * 0.004,

                floatOffset:

                    Math.random()

                    *

                    Math.PI

                    *

                    2

            };


            scene.add(

                mesh

            );


            objects.push(

                mesh

            );

        }


        /* Create 3D decorations */

        for (

            let i = 0;

            i < 35;

            i++

        ) {

            createObject();

        }


        /* =========================

           CENTRAL 3D OBJECT

        ========================= */

        const group = new THREE.Group();


        scene.add(

            group

        );


        const mainGeometry =

            new THREE.TorusKnotGeometry(

                1,

                0.28,

                120,

                16

            );


        const mainMaterial =

            new THREE.MeshStandardMaterial({

                color: 0xffb7d0,

                roughness: 0.3,

                metalness: 0.1

            });


        const mainObject =

            new THREE.Mesh(

                mainGeometry,

                mainMaterial

            );


        group.add(

            mainObject

        );


        /* Decorative rings */

        const ringGeometry =

            new THREE.TorusGeometry(

                1.7,

                0.03,

                16,

                100

            );


        const ringMaterial =

            new THREE.MeshBasicMaterial({

                color: 0xb9d8ff

            });


        const ring =

            new THREE.Mesh(

                ringGeometry,

                ringMaterial

            );


        ring.rotation.x =

            Math.PI / 3;


        group.add(

            ring

        );


        group.position.set(

            3.5,

            0,

            0

        );


        /* =========================

           MOUSE MOVEMENT

        ========================= */

        let mouseX = 0;

        let mouseY = 0;


        window.addEventListener(

            "mousemove",

            (event) => {

                mouseX =

                    (

                        event.clientX

                        /

                        window.innerWidth

                        -

                        0.5

                    )

                    *

                    2;


                mouseY =

                    -

                    (

                        event.clientY

                        /

                        window.innerHeight

                        -

                        0.5

                    )

                    *

                    2;

            }

        );


        /* =========================

           ANIMATION

        ========================= */

        function animate() {

            requestAnimationFrame(

                animate

            );


            /* Main object */

            mainObject.rotation.x += 0.005;

            mainObject.rotation.y += 0.007;


            ring.rotation.z += 0.003;


            /* Floating objects */

            objects.forEach(

                (object) => {

                    object.rotation.x +=

                        object.userData.speed;


                    object.rotation.y +=

                        object.userData.speed;


                    object.position.y +=

                        Math.sin(

                            Date.now()

                            *

                            0.001

                            +

                            object.userData.floatOffset

                        )

                        *

                        0.002;

                }

            );


            /* Mouse interaction */

            group.rotation.y +=

                (

                    mouseX * 0.4

                    -

                    group.rotation.y

                )

                *

                0.03;


            group.rotation.x +=

                (

                    mouseY * 0.2

                    -

                    group.rotation.x

                )

                *

                0.03;


            renderer.render(

                scene,

                camera

            );

        }


        animate();


        /* =========================

           RESPONSIVE

        ========================= */

        window.addEventListener(

            "resize",

            () => {

                camera.aspect =

                    window.innerWidth

                    /

                    window.innerHeight;


                camera.updateProjectionMatrix();


                renderer.setSize(

                    window.innerWidth,

                    window.innerHeight

                );

            }

        );

    </script>

</body>
</html>

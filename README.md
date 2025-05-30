<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Farmacia Nieto - Elaboración Magistral Personalizada</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
            background-color: #f8f9fa;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header */
        header {
            background: linear-gradient(135deg, #2c5530, #4a8b3a);
            color: white;
            padding: 1rem 0;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }

        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
            flex-wrap: wrap;
        }

        .logo h1 {
            font-size: 2.5rem;
            font-weight: bold;
            margin-bottom: 0.5rem;
        }

        .logo p {
            font-size: 1.1rem;
            opacity: 0.9;
        }

        .contact-info {
            text-align: right;
            font-size: 0.9rem;
        }

        .contact-info div {
            margin-bottom: 0.3rem;
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(76, 139, 58, 0.8), rgba(44, 85, 48, 0.8)), 
                        url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 600"><rect fill="%234a8b3a" width="1200" height="600"/><path fill="%23ffffff" opacity="0.1" d="M0,300 Q300,200 600,300 T1200,300 V600 H0 Z"/></svg>');
            background-size: cover;
            background-position: center;
            color: white;
            padding: 4rem 0;
            text-align: center;
        }

        .hero h2 {
            font-size: 3rem;
            margin-bottom: 1rem;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
        }

        .hero p {
            font-size: 1.3rem;
            max-width: 800px;
            margin: 0 auto 2rem;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.3);
        }

        .professional-info {
            background: rgba(255,255,255,0.1);
            padding: 1.5rem;
            border-radius: 10px;
            margin: 2rem auto;
            max-width: 600px;
            backdrop-filter: blur(10px);
        }

        .professional-info h3 {
            font-size: 1.5rem;
            margin-bottom: 0.5rem;
        }

        /* Services Section */
        .services {
            padding: 4rem 0;
            background: white;
        }

        .services h2 {
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 3rem;
            color: #2c5530;
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }

        .service-card {
            background: #f8f9fa;
            padding: 2rem;
            border-radius: 15px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            border-left: 5px solid #4a8b3a;
        }

        .service-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 25px rgba(0,0,0,0.15);
        }

        .service-card h3 {
            color: #2c5530;
            font-size: 1.3rem;
            margin-bottom: 1rem;
        }

        .service-card p {
            color: #666;
            line-height: 1.6;
        }

        /* Contact Section */
        .contact {
            background: linear-gradient(135deg, #2c5530, #4a8b3a);
            color: white;
            padding: 4rem 0;
            text-align: center;
        }

        .contact h2 {
            font-size: 2.5rem;
            margin-bottom: 2rem;
        }

        .contact-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin-top: 2rem;
        }

        .contact-item {
            background: rgba(255,255,255,0.1);
            padding: 1.5rem;
            border-radius: 10px;
            backdrop-filter: blur(10px);
        }

        .contact-item h4 {
            font-size: 1.2rem;
            margin-bottom: 1rem;
        }

        /* Footer */
        footer {
            background: #1a3d1f;
            color: white;
            padding: 3rem 0 1rem;
        }

        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            margin-bottom: 2rem;
        }

        .footer-section h4 {
            font-size: 1.3rem;
            margin-bottom: 1rem;
            color: #4a8b3a;
        }

        .footer-section p {
            margin-bottom: 0.5rem;
            line-height: 1.6;
        }

        .footer-bottom {
            text-align: center;
            padding-top: 2rem;
            border-top: 1px solid #4a8b3a;
            opacity: 0.8;
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                text-align: center;
            }

            .contact-info {
                text-align: center;
                margin-top: 1rem;
            }

            .hero h2 {
                font-size: 2rem;
            }

            .hero p {
                font-size: 1.1rem;
            }

            .services-grid {
                grid-template-columns: 1fr;
            }

            .logo h1 {
                font-size: 2rem;
            }
        }

        /* Animations */
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .service-card {
            animation: fadeInUp 0.6s ease forwards;
        }

        .service-card:nth-child(2) { animation-delay: 0.1s; }
        .service-card:nth-child(3) { animation-delay: 0.2s; }
        .service-card:nth-child(4) { animation-delay: 0.3s; }
        .service-card:nth-child(5) { animation-delay: 0.4s; }
        .service-card:nth-child(6) { animation-delay: 0.5s; }
        .service-card:nth-child(7) { animation-delay: 0.6s; }
        .service-card:nth-child(8) { animation-delay: 0.7s; }
        .service-card:nth-child(9) { animation-delay: 0.8s; }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container">
            <div class="header-content">
                <div class="logo">
                    <h1>Farmacia Nieto</h1>
                    <p>Tu camino hacia el bienestar desde 1996</p>
                </div>
                <div class="contact-info">
                    <div>📱 WhatsApp: (+54) 291432-7031</div>
                    <div>✉️ farmacia.nieto@hotmail.com</div>
                    <div>📍 Bahía Blanca, Buenos Aires</div>
                    <div>⏰ Lun-Vie: 8:00-20:00 | Sáb: 8:00-13:00</div>
                </div>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="container">
            <h2>Elaboración Magistral Personalizada</h2>
            <p>Bajo la dirección técnica de Patricia Victoria Nieto, farmacéutica con una larga trayectoria, te ofrecemos productos de calidad y una atención de excelencia personalizada para cuidar tu salud.</p>
            
            <div class="professional-info">
                <h3>🎓 Farmacéutica Profesional</h3>
                <p>Formulaciones personalizadas según las necesidades específicas de cada paciente</p>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section class="services">
        <div class="container">
            <h2>Nuestros Servicios Especializados</h2>
            
            <div class="services-grid">
                <div class="service-card">
                    <h3>🧬 Medicina Ortomolecular</h3>
                    <p>Tratamientos personalizados basados en el equilibrio molecular óptimo para restaurar la salud natural del organismo.</p>
                </div>

                <div class="service-card">
                    <h3>💆‍♀️ Dermocosmética Especializada</h3>
                    <p>Productos especializados para el cuidado de la piel, formulados específicamente para cada tipo y necesidad.</p>
                </div>

                <div class="service-card">
                    <h3>🌿 Homeopatía</h3>
                    <p>Preparaciones homeopáticas tradicionales elaboradas con los más altos estándares de calidad y pureza.</p>
                </div>

                <div class="service-card">
                    <h3>💊 Medicina Alopática</h3>
                    <p>Medicamentos alopáticos preparados magistralmente según prescripción médica con máxima precisión.</p>
                </div>

                <div class="service-card">
                    <h3>🌱 Fitoterapia</h3>
                    <p>Tratamientos naturales a base de plantas medicinales, respaldados por la tradición y la ciencia moderna.</p>
                </div>

                <div class="service-card">
                    <h3>🌸 Florales de Bach</h3>
                    <p>Esencias florales de Bach y otros sistemas para el equilibrio emocional y el bienestar integral.</p>
                </div>

                <div class="service-card">
                    <h3>🦠 Probióticos</h3>
                    <p>Formulaciones probióticas específicas para restaurar y mantener el equilibrio de la flora intestinal.</p>
                </div>

                <div class="service-card">
                    <h3>⚖️ Hormonas Bioidénticas</h3>
                    <p>Terapias hormonales personalizadas con hormonas bioidénticas para el equilibrio hormonal natural.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section class="contact">
        <div class="container">
            <h2>Contactanos</h2>
            <p>Para más asesoramiento y consultas, comunicate con nosotros. ¡Cuidamos de ti de manera personalizada!</p>
            
            <div class="contact-grid">
                <div class="contact-item">
                    <h4>📞 Teléfono</h4>
                    <p>(+54) 291432-7031</p>
                </div>
                <div class="contact-item">
                    <h4>📧 Email</h4>
                    <p>farmacia.nieto@hotmail.com</p>
                </div>
                <div class="contact-item">
                    <h4>📍 Ubicación</h4>
                    <p>Bahía Blanca, Buenos Aires, Argentina</p>
                </div>
                <div class="contact-item">
                    <h4>🕐 Horarios</h4>
                    <p>Lun-Vie: 8:00-20:00<br>Sáb: 8:00-13:00</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-section">
                    <h4>Farmacia Nieto</h4>
                    <p>Tu camino hacia el bienestar desde 1996.</p>
                    <p>Elaboración magistral personalizada con la más alta calidad.</p>
                    <p>Comprometidos con tu salud y bienestar.</p>
                </div>

                <div class="footer-section">
                    <h4>Nuestros Servicios</h4>
                    <p>Medicina Ortomolecular</p>
                    <p>Dermocosmética Especializada</p>
                    <p>Homeopatía y Alopatía</p>
                    <p>Fitoterapia Natural</p>
                    <p>Florales de Bach</p>
                    <p>Probióticos y Hormonas Bioidénticas</p>
                </div>

                <div class="footer-section">
                    <h4>Información de Contacto</h4>
                    <p>📱 WhatsApp: (+54) 291432-7031</p>
                    <p>✉️ farmacia.nieto@hotmail.com</p>
                    <p>📍 Bahía Blanca, Buenos Aires, Argentina</p>
                    <p>⏰ Lun-Vie: 8:00-20:00 | Sáb: 8:00-13:00</p>
                </div>

                <div class="footer-section">
                    <h4>Dirección Profesional</h4>
                    <p>Directora Técnica: Patricia Victoria Nieto</p>
                    <p>Matrícula Profesional Habilitada</p>
                    <p>28+ años de experiencia</p>
                    <p>Especialista en Elaboración Magistral</p>
                    <p>Universidad Nacional</p>
                </div>
            </div>

            <div class="footer-bottom">
                <p>&copy; 2025 Farmacia Nieto. Todos los derechos reservados. | Elaboración Magistral Personalizada</p>
            </div>
        </div>
    </footer>
</body>
</html>

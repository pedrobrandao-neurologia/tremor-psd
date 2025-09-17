TremorPSD - Análise de Tremor por Acelerometria
Mostrar Imagem Mostrar Imagem Mostrar Imagem Mostrar Imagem

Aplicação web para análise profissional de tremor usando o acelerômetro de dispositivos móveis
Professional web application for tremor analysis using mobile device accelerometers

🇧🇷 Português
Sobre o Projeto
O TremorPSD é uma ferramenta médica inovadora que utiliza o acelerômetro integrado em smartphones e tablets para realizar análise espectral de tremores. A aplicação processa os dados de movimento em tempo real e fornece classificação automática baseada em características de frequência.
Funcionalidades Principais

Coleta de Dados: Captura dados do acelerômetro em alta frequência (50-60 Hz)
Análise Espectral: Realiza FFT (Fast Fourier Transform) para análise de frequência
Classificação Automática: Identifica tipos de tremor baseado em padrões espectrais
Visualização: Gráficos em tempo real do sinal temporal e espectro de frequência
Exportação: Permite exportar dados coletados em formato CSV
Interface Responsiva: Otimizada para dispositivos móveis e tablets

Tipos de Tremor Analisados

Tremor Ortostático (13-18 Hz)

Tremor de alta frequência
Ocorre em posição ortostática
Alto índice de proeminência espectral


Tremor Essencial (4-12 Hz)

Tremor de ação mais comum
Frequência típica entre 6-8 Hz
Pode afetar mãos, cabeça ou voz


Tremor Distônico (4-7 Hz)

Associado à distonia
Espectro mais amplo
Frequência variável


Mioclonia (>3 Hz de largura)

Movimentos involuntários súbitos
Espectro irregular e amplo
Baixa proeminência



Como Usar
Pré-requisitos

Smartphone ou tablet com acelerômetro
Navegador moderno (Chrome, Safari, Firefox)
Conexão HTTPS (necessária para acessar sensores)

Passo a Passo

Abra a aplicação em https://seu-usuario.github.io/tremor-psd/
Permita o acesso aos sensores quando solicitado
Configure a duração da coleta (10-60 segundos)
Escolha o componente do sinal (magnitude total recomendada)
Posicione o dispositivo na área de interesse (mão, braço, etc.)
Toque em "Iniciar Coleta"
Mantenha o dispositivo estável durante a coleta
Visualize os resultados da análise
Exporte os dados se necessário

Métricas Calculadas

Frequência do Pico: Frequência dominante do tremor
Proeminência: Relação entre pico e média espectral
Largura: Largura do pico principal (FWHM)
Taxa de Amostragem: Frequência de coleta dos dados

Instalação e Deploy
GitHub Pages

Crie um repositório no GitHub
Faça upload do arquivo como index.html
Ative GitHub Pages nas configurações
Acesse via https://usuario.github.io/repositorio/

Hospedagem Local
bash# Servidor simples com Python
python -m http.server 8000 --bind 127.0.0.1

# Acesse em https://127.0.0.1:8000
Limitações e Considerações

Não substitui avaliação médica: Esta ferramenta é auxiliar ao diagnóstico
Precisão limitada: Acelerômetros móveis têm limitações de precisão
Contexto clínico: Resultados devem ser interpretados por profissionais
Validação necessária: Algoritmos precisam validação clínica adicional

Tecnologias Utilizadas

HTML5 Canvas para visualização
JavaScript nativo para processamento
CSS3 para interface responsiva
Device Motion API para sensores
FFT personalizada para análise espectral


🇺🇸 English
About the Project
TremorPSD is an innovative medical tool that utilizes built-in accelerometers in smartphones and tablets to perform spectral analysis of tremors. The application processes movement data in real-time and provides automatic classification based on frequency characteristics.
Key Features

Data Collection: Captures accelerometer data at high frequency (50-60 Hz)
Spectral Analysis: Performs FFT (Fast Fourier Transform) for frequency analysis
Automatic Classification: Identifies tremor types based on spectral patterns
Visualization: Real-time graphs of temporal signal and frequency spectrum
Export: Allows exporting collected data in CSV format
Responsive Interface: Optimized for mobile devices and tablets

Analyzed Tremor Types

Orthostatic Tremor (13-18 Hz)

High-frequency tremor
Occurs in orthostatic position
High spectral prominence index


Essential Tremor (4-12 Hz)

Most common action tremor
Typical frequency between 6-8 Hz
May affect hands, head, or voice


Dystonic Tremor (4-7 Hz)

Associated with dystonia
Broader spectrum
Variable frequency


Myoclonus (>3 Hz width)

Sudden involuntary movements
Irregular and broad spectrum
Low prominence



How to Use
Prerequisites

Smartphone or tablet with accelerometer
Modern browser (Chrome, Safari, Firefox)
HTTPS connection (required for sensor access)

Step by Step

Open the application at https://your-username.github.io/tremor-psd/
Allow sensor access when prompted
Configure collection duration (10-60 seconds)
Choose signal component (total magnitude recommended)
Position device on area of interest (hand, arm, etc.)
Tap "Start Collection"
Keep device stable during collection
View analysis results
Export data if needed

Calculated Metrics

Peak Frequency: Dominant tremor frequency
Prominence: Ratio between peak and spectral average
Width: Main peak width (FWHM)
Sample Rate: Data collection frequency

Installation and Deployment
GitHub Pages

Create a GitHub repository
Upload file as index.html
Enable GitHub Pages in settings
Access via https://username.github.io/repository/

Local Hosting
bash# Simple server with Python
python -m http.server 8000 --bind 127.0.0.1

# Access at https://127.0.0.1:8000
Limitations and Considerations

Does not replace medical evaluation: This tool assists diagnosis
Limited accuracy: Mobile accelerometers have precision limitations
Clinical context: Results should be interpreted by professionals
Validation needed: Algorithms require additional clinical validation

Technologies Used

HTML5 Canvas for visualization
Native JavaScript for processing
CSS3 for responsive interface
Device Motion API for sensors
Custom FFT for spectral analysis


📊 Technical Specifications
System Requirements

Mobile OS: iOS 13+ or Android 7+
Browsers: Chrome 80+, Safari 13+, Firefox 75+
Sensors: 3-axis accelerometer required
Network: HTTPS connection mandatory

Data Processing Pipeline

Acquisition: Raw accelerometer data (x, y, z axes)
Preprocessing: DC removal and signal conditioning
Spectral Analysis: FFT computation and power spectrum
Feature Extraction: Peak detection and metrics calculation
Classification: Heuristic-based tremor type identification

File Structure
tremor-psd/
├── index.html          # Main application file
├── README.md           # This documentation
└── sw.js               # Service worker (embedded)
📄 License
This project is for educational and research purposes. Not intended for clinical diagnosis without proper validation.
🤝 Contributing
Contributions are welcome! Please ensure any medical algorithms are properly validated and documented.
⚠️ Disclaimer
This application is a research tool and should not be used as the sole basis for medical diagnosis. Always consult qualified healthcare professionals for proper tremor evaluation and treatment.

# 🤖 Xatbot IPOP
## 📖 Descripció
Xatbot intel·ligent que s'integra a un portfoli en WordPress i respon segons la informació de la web personal.

Permet personalitzar el comportament del xatbot, fer web scraping i millorar el model mitjançant API.
## 🎯 Objectius
1. Desenvolupar un xatbot que respongui segons el contingut d'una web.
2. Integrar-lo a WordPress com un widget.
3. Fer servir Google Gemini API per generar respostes.
4. Aprendre a gestionar API Keys i seguretat bàsica.
5. Utilitzar web scraping per extreure informació d'una pàgina.
## 📦 Requisits
Abans d’iniciar el projecte, assegura’t de tenir instal·lats:

1. Python 3.x (python --version)
2. Google Gemini API Key (Obtenir-la a Google AI Studio)
3. Google Colab o entorn local amb biblioteques necessàries
4. Un entorn de proves per al frontend (Google Sites, WordPress, etc.)
## 📂 Estructura del projecte
📦 xatbot-ipop 
1. ┣ 📂 src # Codi font del backend ┃ 
2. ┣ 📜 main.ipynb # Backend principal del xatbot ┃ 
3. ┣ 📜 chatbot.ipynb # Lògica del chatbot (instruccions, API) ┃ 
4. ┣ 📜 scraper.ipynb # Web scraping per extreure informació ┃ 
5. ┗ 📜 config.ipynb # Configuració de la API i altres paràmetres 

6. ┣ 📂 frontend # Widget frontend (HTML, CSS, JS) ┃ 
7. ┗ 📜 index.html # Integració al WordPress 

8. ┣ 📂 docs # Documentació del projecte 
9. ┣ 📜 requirements.txt # Biblioteques necessàries 
10. ┣ 📜 README.md # Aquest fitxer 
11. ┣ 📜 CHANGELOG.md # Registre de versions i canvis 
12. ┗ 📜 CONTRIBUTING.md # Guia per col·laboradors

## 🔧 Instal·lació

1️⃣. Instal·lació de biblioteques i mòduls (Backend)
2️⃣. Configuració de l’API Key
3️⃣. Executar el xatbot


## 🔁 Fluxe de dades

🔽 El backend processa la consulta de l’usuari.
🔽 Recull informació del WordPress (opcional, via web scraping).
🔽 Envia la resposta generada pel model cap al frontend.
🔽 El frontend mostra la resposta a l’usuari en un widget.

## 👨‍💻 Contribució
Si vols contribuir, segueix les normes indicades a CONTRIBUTING.md.

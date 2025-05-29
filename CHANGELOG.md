📄 Registre de canvis (Changelog)
✅ Versió 0.1.0 - Versió mínima funcional

    Es crea un servidor Flask amb una única ruta /chatbot.

    S'implementa una funció bàsica de scraping d'una pàgina web amb requests i BeautifulSoup.

    El bot utilitza l'API de Gemini (Google) per respondre preguntes combinant el contingut web amb el missatge de l'usuari.

    Configuració de la clau API a través de userdata.

🔧 Versió 0.2.0 - Connectivitat i exposició del servei

    Integració amb Ngrok per exposar el port 5000 públicament.

    Automatització del tancament de processos que utilitzen el port 5000 (!kill -9 $(lsof -t -i:5000)).

    Impressió automàtica de la URL pública per facilitar l'accés remot.

🛡 Versió 0.3.0 - Millores de seguretat i estabilitat

    S'afegeix control d'errors a la petició requests.get() amb try/except i raise_for_status().

    Gestió de l'excepció si la pàgina no té títol.

    Es verifica la presència de la clau API i es para el programa si no està configurada.

    Reducció del temps d'espera de les peticions web (timeout=1) per evitar bloquejos llargs.

🌐 Versió 0.4.0 - CORS i API més robusta

    S'afegeix suport complet per a CORS, permetent peticions des de qualsevol domini.

    Millora de la resposta d'error quan no es proporciona cap missatge en la sol·licitud al endpoint /chatbot.

    S'afegeix un middleware @after_request per configurar correctament les capçaleres CORS en totes les respostes.

🧠 Versió 0.5.0 - Millora de l’experiència del chatbot

    Es configura el model de Gemini amb paràmetres personalitzats: temperature=0.7 i max_output_tokens=200.

    S'afegeix una instrucció de sistema al model per personalitzar l'estil de les respostes (evitant preguntes personals o no relacionades amb la web).

    El codi es reorganitza amb comentaris estructurats per millorar-ne la llegibilitat i mantenibilitat.


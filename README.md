Introducere

Prin această aplicație mi-am propus ca fiecare utilizator să aibă posibilitatea să vadă vremea din orice oraș din orice țară folosind un API de API weather. De asemenea, aplicația are un API de login unde am folosit Amazon Web Services (AWS).
Descriere problemă
Această aplicație ajută userii să vadă vremea din orice oraș își doresc într-un timp util și rapid. Am încercat să realizez și o pagină de conectare pentru această aplicație web.

Descriere API 

OpenWeatherMap este un serviciu online care oferă date meteorologice, inclusiv date meterorlogice curente, prognoze și date și date istorice dezvoltatorilor de servicii web și aplicații mobile. Pentru sursele de date, utilizează servicii de difuzare meteorologică, date brute de la stațiile meteo din aeroport, date brute de la stațiile radar și date brute de la alte stații meteorologice oficiale. Toate datele sunt prelucrate de OpenWeatherMap într-un mod în care încearcă să furnizeze date precise de prognoză online și hărți meteo, cum ar fi cele pentru nori sau precipitații. Dincolo de asta, serviciul este axat pe aspectul social, implicând proprietarii stațiilor meteo în conectarea la acest serviciu și, prin urmare, creșterea preciziei datelor meteo.

OpenWeatherMap oferă o API cu puncte finale JSON, XML și HTML, dar și un nivel de utilizare gratuită limitat.





Amazon Web Services (AWS)
Acest API a folosit pentru login la service-ul de backend pentru auth. Acesta este o filială a Amazonului care furnizează platforme și API-uri de cloud computing la cerere pentru persoane fizice, pe bază de plată măsurată. Aceste servicii web de cloud computing oferă o varietate de infrastructuri tehnice abstracte de bază și blocuri și instrumente de calcul distribuite. Unul dintre aceste servicii este Amazon Elastic Compute Cloud (EC2, care permite utilizatorilor să aibă la dispoziție un cluster virtual de computere, disponibile tot timpul prin Internet. Versiunea AWS a computerelor virtuale emulează majoritatea atributelor unui computer real, inclusiv centrale de procesare hardware.

Tehnologia AWS este implementată la fermele de servere din întreaga lume și este întreținută de filiala Amazon. Taxele se bazează pe modelul de plată Pay-as-you-go, având sistemul de operare, HW și software sau caracteristici de rețea alese de abonat, disponibilitate, redundanță, securitate și opțiuni de servicii necesare. Abonații pot plăti pentru un singur computer AWS. Acesta funcționează din multe regiuni geografice globale, inclusiv 6 din America de Nord

În 2006, AWS a început să ofere servicii de infrastructură IT companiilor sub formă de servicii web - cunoscute în prezent sub denumirea de cloud computing. Unul dintre beneficiile cheie ale cloud computingului este oportunitatea de a înlocui cheltuielile de infrastructură de capital inițiale cu costuri variabile mici. Cu cloud, companiile nu mai trebuie să planifice și să achiziționeze servere cu luni în avans.

Astăzi, AWS oferă o platformă de infrastructură extrem de scalabilă, cu costuri reduse, utilizată în peste 190 de țări din întreaga lume.





Flux de date
Fluxul de date este evidențiat prin următorul parcurs. Primul pas pe care îl face orice user pentru a utiliza aplicația trebuie, în primul rând să își creeze un cont. După urmează partea de login ce implică o parte de validare. Dacă un user fără cont încearcă să se logheze nu va reuși (un error message o să specifice acest lucru), urmând să fie evidențiată pagina web în care poate fi verificată vremea din orice oraș prin API-ul de OpenWeatherMap.
De specificat este că datele din register sunt salvate în baza de date ofertă de cloud.


Metode HTTP
Am utilizat fetch pentru a realiza conexiunea cu API-ul care ne oferă date privind vremea orașelor din toată lumea.

Autentificare și autorizare servicii utilizate
Am realizat un serviciu de autentificare cu ajutorul AWS auth. Acesta a fost urcat pe un domein (https://main.d2wcsctjr5vox8.amplifyapp.com/), însă aici nu am reușit să configurez partea de back-end pentru a crea un cont, a mă loga pentru a utiliza aplicația de weather. Astfel, aplicația (fără login) este disponibilă pe link-ul https://master.d2qcjpsw9tkmzu.amplifyapp.com/

Capturi de ecran:

Figura 1 - Sign in


Fig.2 Sign up


Fig.3 Main App




Fig.4 App.js - code


Fig.5 Weather code app

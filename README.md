<html>
      <head>
            <meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
	  <title>Übung Verzweigung</title>
		
	  <script>
			"use strict";

			function clicked() {
			let Umsatz = document.getElementById("idUmsatz").value;
			let ausgabe = "Prämie : " + fPrämie(Umsatz); 
			document.getElementById("idAusgabe").innerHTML = ausgabe;

			}
			
			function fPrämie (Umsatz) {

			if (Umsatz<50000) {return "Sie bekommen Nix"} 
			else if (Umsatz<100000) {return "Sie bekommen einen Blumenstrauß"}
			else if (Umsatz<150000) {return "Sie bekommen einen Buchgutschein "}
			else {return " Sie bekommen eine Reise "}
					
			}

	  </script>
	  </head>

	  <body>
		<h1>Jahresumsatz - Prämie</h1>
		Jahresumsatz <input id="idUmsatz" type="text" value="25"><br><br>
		<button onclick="clicked();">Prämie!</button><br><br>
		<div id="idAusgabe">Hier kommt beim Klicken auf den Button eine Ausgabe.</div>
	

       </body>
</html>

  

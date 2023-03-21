<!DOCTYPE html>
<html>
<head>
	<title>Benutzerdaten</title>
</head>
<body>
	<h1>Benutzerdaten</h1>

	<!-- Formular zum Hinzufügen neuer Benutzerdaten -->
	<form method="post" action="<?php echo $_SERVER['PHP_SELF']; ?>">
		<label for="benutzername">Benutzername:</label>
		<input type="text" name="benutzername" required><br><br>
		<label for="email">Email:</label>
		<input type="email" name="email" required><br><br>
		<input type="submit" value="Hinzufügen">
	</form>

	<?php
	// Verbindung zur Datenbank herstellen
	$servername = "localhost";
	$username = "root";
	$password = "";
	$dbname = "benutzerdaten";

	$conn = new mysqli($servername, $username, $password, $dbname);

	// Überprüfen, ob die Verbindung erfolgreich hergestellt wurde
	if ($conn->connect_error) {
	    die("Verbindung fehlgeschlagen: " . $conn->connect_error);
	}

	// Neue Benutzerdaten in die Datenbank einfügen, wenn das Formular abgesendet wurde
	if ($_SERVER["REQUEST_METHOD"] == "POST") {
		$benutzername = $_POST["benutzername"];
		$email = $_POST["email"];

		$sql = "INSERT INTO benutzer (benutzername, email) VALUES ('$benutzername', '$email')";

		if ($conn->query($sql) === TRUE) {
			echo "<p>Benutzerdaten erfolgreich hinzugefügt.</p>";
		} else {
			echo "<p>Fehler beim Hinzufügen der Benutzerdaten: " . $conn->error . "</p>";
		}
	}

	// Alle in der Datenbank vorhandenen Benutzer abrufen und anzeigen
	$sql = "SELECT * FROM benutzer";
	$result = $conn->query($sql);

	if ($result->num_rows > 0) {
		echo "<h2>Alle Benutzer:</h2>";
		echo "<ul>";
		while($row = $result->fetch_assoc()) {
			echo "<li>" . $row["benutzername"] . " (" . $row["email"] . ")</li>";
		}
		echo "</ul>";
	} else {
		echo "<p>Keine Benutzerdaten vorhanden.</p>";
	}

	// Verbindung zur Datenbank schließen
	$conn->close();
	?>
</body>
</html>

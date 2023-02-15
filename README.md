<!DOCTYPE html>
<html lang="es">
<head>
	<meta charset="UTF-8">
	<title>Presentación de Tecnologías</title>
	<style>
		/* Estilos para la presentación */
		body {
			font-family: sans-serif;
			max-width: 800px;
			margin: 0 auto;
			padding: 2rem;
		}

		h1, h2 {
			text-align: center;
		}

		ul {
			list-style: none;
			margin: 0;
			padding: 0;
			display: flex;
			justify-content: center;
			align-items: center;
		}

		li {
			margin: 1rem;
			padding: 1rem;
			background-color: #eee;
			border-radius: 0.5rem;
			box-shadow: 0 0 0.5rem rgba(0, 0, 0, 0.3);
		}

	</style>
</head>
<body>
	<h1>Presentación de Tecnologías</h1>
	<h2>Por <span id="nombre"></span></h2>
	<ul id="tecnologias">
		<!-- Las tecnologías se agregarán con JavaScript -->
	</ul>
	<script>
		// Agrega el nombre del presentador
		document.getElementById("nombre").textContent = "Tu Nombre";

		// Agrega las tecnologías
		const tecnologias = ["HTML", "CSS", "JavaScript", "React", "Node.js"];
		const lista = document.getElementById("tecnologias");

		tecnologias.forEach(tecnologia => {
			const item = document.createElement("li");
			item.textContent = tecnologia;
			lista.appendChild(item);
		});
	</script>
</body>
</html>

# angularjs
Controller
<!DOCTYPE html>
<html lang="" ng-app="minmax">
	<head>
		<meta charset="utf-8">
		<meta http-equiv="X-UA-Compatible" content="IE=edge">
		<meta name="viewport" content="width=device-width, initial-scale=1">
		<title>Contoler</title>

		<!-- Bootstrap CSS -->
		<link href="css/bootstrap.min.css" rel="stylesheet">

		<!-- HTML5 Shim and Respond.js IE8 support of HTML5 elements and media queries -->
		<!-- WARNING: Respond.js doesn't work if you view the page via file:// -->
		<!--[if lt IE 9]>
			<script src="https://oss.maxcdn.com/libs/html5shiv/3.7.0/html5shiv.js"></script>
			<script src="https://oss.maxcdn.com/libs/respond.js/1.4.2/respond.min.js"></script>
		<![endif]-->
	</head>
	<body>
	
	<nav class="navbar navbar-inverse">
		<a class="navbar-brand" href="#">Anugularjs </a>
		<ul class="nav navbar-nav">
			<li class="active">
				<a href="#">Controler</a>
			</li>
			
		</ul>
	</nav>

		<div class="container main-content" ng-controller="MinMaxCntrol">
		 <form>
		 	<div class="form-group">
		 		<label for="name">Name</label>
		 		<input type="text" class="form-control"  ng-model="formModel.name" placeholder="Name" id="name">
		 	</div>

		 	<div class="form-group">
		 		<label for="Email">Email</label>
		 		<input type="email" class="form-control" ng-model="formModel.email"  placeholder="Email" id="email">
		 	</div>

		 	<div class="form-group">
		 		<label for="password">Password</label>
		 		<input type="password" class="form-control" ng-model="formModel.password"  placeholder="Password" id="password">
		 	</div>
				
			<div class="form-group">
				<button class="btn btn-primary" ng-click="onSubmit()">Register</button>
			</div>

		 </form>

		 <pre>{{ formModel | json}}	</pre>		

		</div>



		<!-- jQuery -->
		<script src="js/jquery.min.js"></script>
		<!-- Bootstrap JavaScript -->
		<script src="js/bootstrap.min.js"></script>
		<!-- Angularjs -->
		<script src="js/angular.min.js"></script>

		<script src="main.js"></script>
	</body>
</html>

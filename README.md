# projetoangular
Treinamento de um Projeto criado em AngularJS


Escopo base para a criação inicial de um projeto

<!DOCTYPE html>
<html ng-app="helloWorld">
<head>
    <title>Hello World</title>
    <script src="angular.js"></script>
    <script>
        angular.module("helloWorld", []);
        angular.module("helloWorld").controller("helloWorldCtrl", function ($scope) {
            $scope.message = "Ola Mundo, estou de volta!";
        })
    </script>
</head>
<body>
    <div ng-controller="helloWorldCtrl">
       <h1>{{message}}</h1> 
    </div>
</body>
</html>

ng-app = Define as fronteiras da aplicação
ng-controller = Vincula um elemento da view ao controller
ng-bind = Sustitui o elemento por uma expressão
ng-repeat = faz interação sobre os itens de uma coleção ou de um objeto
ng-model - vincula uma propriedade ao $scope
ng-click = atribui um comportamento ao evento
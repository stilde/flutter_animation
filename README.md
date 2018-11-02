# animation

A new Flutter project.

## Getting Started

### Théorie sur l'animation

Lorsque vous envisagez d'ajouter une animation à votre widget, vous devez créer un contrôleur d'animation dans votre widget Stateful. La classe d'état de ce widget doit être ajoutée à Mixin sous le nom SingleTickerProviderStateMixin . Comme son nom l'indique, il est utilisé lorsque votre widget ne contient qu'un seul contrôleur d'animation et que son travail consiste à fournir une valeur de ticker au widget à état dynamique.

### Qu'est-ce que c'est Ticker ???

Lorsque vous ajoutez votre SingleTickerProviderStateMixin, il indique à Flutter que ce widget contient une animation et que ce widget doit être averti des images d'animation de Flutter.

### Manette

Le contrôleur d’animation est l’un des éléments de base nécessaires pour créer de la magie dans le flutter. Vous pouvez imaginer cela en tant que dictateur de l'animation à l'écran. Il contient la durée de l'animation et il divisera donc les valeurs entre 0 et 1 en fonction de la durée et de la valeur du ticker.

La valeur du contrôleur est 0 -> Début de votre animation

La valeur du contrôleur est 1 -> Fin de votre animation
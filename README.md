Rails app generated with [lewagon/rails-templates](https://github.com/lewagon/rails-templates), created by the [Le Wagon coding bootcamp](https://www.lewagon.com) team.

# Introduction à la gestion des Hash en Ruby

## Plan du cours

### 1. Introduction aux Hash
- Définition et utilisation basique

### 2. Méthodes de base
- `keys`, `values`, `merge`, `delete`

```ruby
my_hash.keys
my_hash.merge({"key3" => "value3"})
my_hash.delete("key1")
```

### 3. Méthodes pour Itération
- Utilisation de `each` pour parcourir un hash

### 4. Vérification de l'Existence
- Utilisation de `has_key?` et `has_value?`

### 5. Méthodes pour Transformation
- `transform_keys` et `transform_values`

### 6. Arguments Optionnels avec Hash
- Exemple simple d'ajout de nombres avec une option

### 7. Symboles
- 9.1 Définition et différence avec les chaînes de caractères
- 9.2 Utilisation comme clés dans les hash
- 9.3 Avantages en termes de performance et d'immuabilité
  - 9.3.1 Performance
  - 9.3.2 Immuabilité
  - 9.3.3 Utilisation en pratique
  - 9.3.4 Cas où la performance est cruciale

### 8. Exercices Pratiques
- Appliquer les méthodes apprises sur des exemples concrets

### 9. Points d'Intérêt et Approfondissement
- Importance de lire la documentation
- Comment et quand utiliser ces méthodes et notions dans des projets réels
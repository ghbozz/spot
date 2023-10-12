Rails app generated with [lewagon/rails-templates](https://github.com/lewagon/rails-templates), created by the [Le Wagon coding bootcamp](https://www.lewagon.com) team.

# Introduction à la gestion des Hash en Ruby

## Plan du cours

### 1. Introduction aux Hash
- Définition et utilisation basique

```ruby
my_hash = {"key1" => "value1", "key2" => "value2"}

# Create: Ajouter des éléments à un hash
my_hash = {}
my_hash[:create] = "Create example"

# Read: Lire un élément d'un hash
read_example = my_hash[:create]

# Update: Modifier un élément d'un hash
my_hash[:create] = "Updated create example"

# Delete: Supprimer un élément d'un hash
my_hash.delete(:create)
```

### 2. Méthodes de base
- `keys`, `values`, `merge`, `delete`

```ruby
my_hash.keys
my_hash.merge({"key3" => "value3"})
my_hash.delete("key1")
```

### 3. Méthodes pour Itération
- Utilisation de `each` pour parcourir un hash

```ruby
my_hash.each {|key, value| puts "#{key}: #{value}"}
```

### 4. Vérification de l'Existence
- Utilisation de `has_key?` et `has_value?`

```ruby
my_hash.has_key?("key1")
my_hash.has_value?("value1")
```

### 5. Méthodes pour Transformation
- `transform_keys` et `transform_values`

```ruby
my_hash.transform_keys(&:upcase)
my_hash.transform_values(&:reverse)
```

### 6. Arguments Optionnels avec Hash
- Exemple simple d'ajout de nombres avec une option

```ruby
def add_numbers(a, b, options = {})
  sum = a + b
  sum *= options[:multiplier] if options[:multiplier]
  sum
end
```

### 7. Symboles
- 9.1 Définition et différence avec les chaînes de caractères
- 9.2 Utilisation comme clés dans les hash
- 9.3 Avantages en termes de performance et d'immuabilité
  - 9.3.1 Performance
  - 9.3.2 Immuabilité
  - 9.3.3 Utilisation en pratique
  - 9.3.4 Cas où la performance est cruciale

```ruby
:my_symbol
"my_string"

symbol_hash = {one: 1, two: 2}
symbol_hash[:one]
```

### 8. Exercices Pratiques
- Appliquer les méthodes apprises sur des exemples concrets

### 9. Points d'Intérêt et Approfondissement
- Importance de lire la documentation
- Comment et quand utiliser ces méthodes et notions dans des projets réels
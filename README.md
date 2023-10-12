Rails app generated with [lewagon/rails-templates](https://github.com/lewagon/rails-templates), created by the [Le Wagon coding bootcamp](https://www.lewagon.com) team.

# Introduction à la gestion des Hash en Ruby

## Plan du cours

### 1. Introduction aux Hash
- Définition et utilisation basique

```ruby
user_data = {"key1" => "value1", "key2" => "value2"}

# Create: Créer un hash pour un nouvel utilisateur avec des clés en chaînes
user_data_string = {}
user_data_string["name"] = "Alice"
user_data_string["age"] = 30

# Create: Avec des clés en symboles
user_data_symbol = {}
user_data_symbol[:name] = "Alice"
user_data_symbol[:age] = 30

# Read: Lire des données à partir du hash (version chaîne)
name_string = user_data_string["name"]

# Read: (version symbole)
name_symbol = user_data_symbol[:name]

# Update: Mettre à jour l'âge de l'utilisateur (version chaîne)
user_data_string["age"] = 31

# Update: (version symbole)
user_data_symbol[:age] = 31

# Delete: Supprimer l'âge de l'utilisateur (version chaîne)
user_data_string.delete("age")

# Delete: (version symbole)
user_data_symbol.delete(:age)
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
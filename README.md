# MongoDB :leaves:
В данном задании с помощью инсрумента MongoDB мною была создана своя база данных с коллекциями, здесь представлены несколько запросов к ним :european_castle:

# Выведите всех персонажей, чей возраст больше 10, но меньше 20 
:heavy_check_mark: db.characters.find({ age: { $gt: 10, $lt: 20 } })

# Выведите всех персонажей, чей возраст меньше 30 и не равен 11
:heavy_check_mark: db.characters.find({ age: { $lt: 30, $ne: 11 } })

# Добавьте всем персонажам 1 год к возрасту
 :heavy_check_mark: db.characters.updateMany({}, { $inc: { age: 1 }})

# Посчитайте общее количество персонажей, чей возраст больше 11
:heavy_check_mark: db.characters.count({age:{$gt:11}})

# Удалите информацию о книге 'Quidditch Through The Ages'
 :heavy_check_mark: db.library.deleteOne( { book_name: " Quidditch Through The Ages" } )

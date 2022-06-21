#HomeWork

скопируйте папку homework_02 для этой домашки (Памятка: https://github.com/OtusTeam/BasePython/tree/homeworks-new)
в модуле exceptions объявите следующие исключения:
LowFuelError
NotEnoughFuel
CargoOverload
доработайте базовый класс base.Vehicle:
добавьте атрибуты weight, started, fuel, fuel_consumption со значениями по умолчанию
добавьте инициализатор для установки weight, fuel, fuel_consumption
добавьте метод start, который, если ещё не состояние started, проверяет, что топлива больше нуля, и обновляет состояние started, иначе выкидывает исключение exceptions.LowFuelError
добавьте метод move, который проверяет, что достаточно топлива для преодоления переданной дистанции, и изменяет количество оставшегося топлива, иначе выкидывает исключение exceptions.NotEnoughFuel
создайте датакласс Engine в модуле engine, добавьте атрибуты volume и pistons
в модуле car создайте класс Car
класс Car должен быть наследником Vehicle
добавьте атрибут engine классу Car
объявите метод set_engine, который принимает в себя экземпляр объекта Engine и устанавливает на текущий экземпляр Car
в модуле plane создайте класс Plane
класс Plane должен быть наследником Vehicle
добавьте атрибуты cargo и max_cargo классу Plane
добавьте max_cargo в инициализатор (переопределите родительский)
объявите метод load_cargo, который принимает число, проверяет, что в сумме с текущим cargo не будет перегруза, и обновляет значение, в ином случае выкидывает исключение exceptions.CargoOverload
объявите метод remove_all_cargo, который обнуляет значение cargo и возвращает значение cargo, которое было до обнуления
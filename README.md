# Childdieseas
class ChildDisease:
    def __init__(self, name, symptoms, age_range, severity="Легкая"):
        self.name = name
        self.symptoms = symptoms
        self.age_range = age_range
        self.severity = severity

    def update_severity(self, new_severity):
        self.severity = new_severity

    def __str__(self):
        return f"Болезнь детского возраста: {self.name} (Симптомы: {', '.join(self.symptoms)}, Возрастная группа: {self.age_range}, Степень тяжести: {self.severity})"

# Пример использования класса ChildDisease
child_disease1 = ChildDisease("Грипп", ["Высокая температура", "Насморк"], "Дошкольники")
print(child_disease1)

child_disease1.update_severity("Средняя")
print(child_disease1)

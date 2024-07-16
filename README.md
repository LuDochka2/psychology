# psychologyimport random

class SubconsciousMind:
    def __init__(self):
        self.thoughts = []

    def receive_input(self, input_text):
        self.thoughts.append(input_text)

    def generate_output(self):
        if self.thoughts:
            return random.choice(self.thoughts)
        else:
            return "No thoughts at the moment."

# Example usage:
subconscious = SubconsciousMind()

# Simulating input
subconscious.receive_input("I feel happy today.")
subconscious.receive_input("What should I have for lunch?")
subconscious.receive_input("I need to finish that project.")

# Generating output
print("Subconscious output:")
for _ in range(3):
    print(subconscious.generate_output())

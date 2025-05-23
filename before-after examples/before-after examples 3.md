Example 3: Input and Menu Handling

Initial Prompt

How can I ask the user for a city name?

Initial AI-Generated Code (Before)

city = input("City: ")

My Analysis

No validation

No default or menu system for ease of use

Doesn’t handle empty input

Follow-up Prompt

Can you improve this so it gives a default city if none is entered and offers a menu of popular options?

Improved Code (After)

popular = ["Perth", "Sydney", "Melbourne"]
print("Select a city or press Enter for default (Perth):")
for i, c in enumerate(popular, 1):
    print(f"{i}. {c}")

choice = input("Enter number or name: ").strip()
if choice.isdigit() and 1 <= int(choice) <= len(popular):
    city = popular[int(choice) - 1]
elif choice:
    city = choice
else:
    city = "Perth"

Why the Prompt Worked

Introduced a specific improvement (usability and defaults)

Resulted in more robust, user-friendly code

# FirstTaskhello
import random

print("Choose a template (type 1, 2, or 3). Type R to pick a random template.")
choice = input("Your choice: ").strip().lower()

if choice == "r":
    template_number = random.choice([1, 2, 3])
else:
    try:
        template_number = int(choice)
        if template_number not in (1, 2, 3):
            print("Invalid number, defaulting to template 1.")
            template_number = 1
    except ValueError:
        print("Invalid input, defaulting to template 1.")
        template_number = 1



# Template 1
if template_number == 1:
    number = input("Input number: ").strip()
    measure_of_time = input("Input measure of time: ").strip()
    mode_of_transportation = input("Input mode of transportation: ").strip()
    adjective = input("Input adjective: ").strip()
    adjective2 = input("Input second adjective: ").strip()
    nouns = input("Input noun(s): ").strip()
    color = input("Input color: ").strip()
    parts_of_body = input("Input part of body(s): ").strip()
    verb = input("Input verb: ").strip()
    number2 = input("Input second number: ").strip()
    noun2s = input("Input second noun(s): ").strip()
    noun3 = input("Input third noun: ").strip()
    part_of_body2 = input("Input second part of body: ").strip()
    noun4 = input("Input fourth noun: ").strip()
    adjective3 = input("Input third adjective: ").strip()
    silly_word = input("Input silly word: ").strip()

    story = (
        f"It was about {number} {measure_of_time} ago when I arrived at the hospital in a {mode_of_transportation}.\n"
        f"The hospital is a {adjective} place; there are a lot of {adjective2} {nouns} here.\n"
        f"There are nurses who have {color} {parts_of_body}.\n"
        f"If someone wants to come into my room I told them that they have to {verb} first.\n"
        f"I've decorated my room with {number2} {noun2s}.\n"
        f"Today I talked to a doctor and they were wearing a {noun3} on their {part_of_body2}.\n"
        f"I heard that all doctors {verb} {noun4} every day for breakfast.\n"
        f"The most {adjective3} thing about being in the hospital is the {silly_word} {nouns}!\n"
    )


# Template 2
elif template_number == 2:
    person_name = input("Input person name: ").strip()
    noun = input("Input noun: ").strip()
    adjective = input("Input adjective: ").strip()
    feeling = input("Input a feeling: ").strip()
    verb = input("Input a verb: ").strip()
    adjective2 = input("Input second adjective: ").strip()
    feeling2 = input("Input second feeling: ").strip()
    animal = input("Input an animal: ").strip()
    verb2 = input("Input second verb: ").strip()
    verb_ing = input("Input verb ending with (ing): ").strip()
    adverb_ily = input("Input adverb ending with (ily): ").strip()
    measure_of_time = input("Input measure of time: ").strip()
    noun2 = input("Input second noun: ").strip()
    silly_word = input("Input silly word: ").strip()
    color = input("Input color: ").strip()
    number = input("Input number: ").strip()

    story = (
        f"This weekend I am going camping with {person_name}.\n"
        f"I packed my lantern, sleeping bag, and {noun}.\n"
        f"I am so {adjective} {feeling} to {verb} in a tent.\n"
        f"I am {adjective2} {feeling2}; we might see a(n) {animal}, I hear they're kind of dangerous.\n"
        f"While we're camping, we are going to hike, fish, and {verb2}.\n"
        f"I have heard that the {color} lake is great for {verb_ing}.\n"
        f"Then we will {adverb_ily} hike through the forest for {number} {measure_of_time}.\n"
        f"If I see a {color} {animal} while hiking, I am going to bring it home as a pet!\n"
        f"At night we will tell {number} {silly_word} stories and roast {noun2} around the campfire.\n"
    )


# Template 3
else:
    person_name = input("Input person name: ").strip()
    adjective = input("Input adjective: ").strip()
    color = input("Input color: ").strip()
    animal = input("Input animal: ").strip()
    place = input("Input place: ").strip()
    adjective2 = input("Input second adjective: ").strip()
    magical_creatures = input("Input magical creature (plural): ").strip()
    adjective3 = input("Input third adjective: ").strip()
    magical_creatures2 = input("Input second magical creature (plural): ").strip()
    room_in_a_house = input("Input a room in a house: ").strip()
    noun = input("Input noun: ").strip()
    noun2 = input("Input second noun: ").strip()
    noun_plural3 = input("Input noun (plural): ").strip()
    noun_plural4 = input("Input another noun (plural): ").strip()
    adjective4 = input("Input fourth adjective: ").strip()
    number = input("Input number: ").strip()
    measure_of_time = input("Input measure of time: ").strip()
    adjective5 = input("Input fifth adjective: ").strip()
    noun5 = input("Input fifth noun: ").strip()
    verb_ing = input("Input verb with (ing): ").strip()

    story = (
        f"Dear {person_name}, I am writing to you from a {adjective} castle in an enchanted forest.\n"
        f"I found myself here one day after going for a ride on a {color} {animal} in {place}.\n"
        f"There are {adjective2} {magical_creatures} and {adjective3} {magical_creatures2} here!\n"
        f"In the {room_in_a_house} there is a pool full of {noun}. I fall asleep each night on a {noun2} of {noun_plural3} and dream of {adjective4} {noun_plural4}.\n"
        f"It feels as though I have lived here for {number} {measure_of_time}.\n"
        f"I hope one day you can visit, although the only way to get here now is {verb_ing} on a {adjective5} {noun5}!\n"
    )

print("\n--- GENERATED STORY ---\n")
print(story)
print("\n--- End ---")

# reposatory

# Question Bank
questions = [
    {"topic": "Volunteering", "difficulty": "Easy", "question": "Which of the following is a common reason people choose to volunteer?", "options": ["Financial gain", "Social recognition", "Personal satisfaction", "Professional requirement"], "correct": 2},
    {"topic": "Volunteering", "difficulty": "Easy", "question": "What is the term for a volunteer who helps organize community events?", "options": ["Coordinator", "Participant", "Supervisor", "Spectator"], "correct": 0},
    {"topic": "Volunteering", "difficulty": "Easy", "question": "Which of the following is typically NOT a benefit of volunteering?", "options": ["Gaining new skills", "Meeting new people", "Receiving a salary", "Helping others"], "correct": 2},
    {"topic": "Volunteering", "difficulty": "Easy", "question": "What type of organization often relies heavily on volunteers?", "options": ["Corporate businesses", "Nonprofits", "Government agencies", "Private schools"], "correct": 1},
    {"topic": "Volunteering", "difficulty": "Easy", "question": "Volunteering at a hospital usually involves helping with:", "options": ["Performing surgeries", "Administrative tasks", "Managing finances", "Legal consultations"], "correct": 1},
    {"topic": "Volunteering", "difficulty": "Moderate", "question": "What is a key motivation for many volunteers, according to studies?", "options": ["Academic credit", "Religious beliefs", "Political influence", "Cultural exchange"], "correct": 1},
    {"topic": "Volunteering", "difficulty": "Moderate", "question": "What is the term for volunteering abroad to help with development projects?", "options": ["Ecotourism", "International aid", "Humanitarianism", "Voluntourism"], "correct": 3},
    {"topic": "Volunteering", "difficulty": "Moderate", "question": "Which organization is known for its emergency disaster response volunteers?", "options": ["Greenpeace", "The Red Cross", "World Wildlife Fund", "Amnesty International"], "correct": 1},
    {"topic": "Volunteering", "difficulty": "Moderate", "question": "What is one of the main challenges faced by volunteer organizations?", "options": ["Excessive funding", "Volunteer burnout", "High employee turnover", "Surplus of volunteers"], "correct": 1},
    {"topic": "Volunteering", "difficulty": "Moderate", "question": "Which of the following skills is often enhanced by volunteering?", "options": ["Archery", "Public speaking", "Financial trading", "Programming"], "correct": 1},
    {"topic": "Volunteering", "difficulty": "Difficult", "question": "Which country has the highest percentage of its population engaged in volunteering?", "options": ["United States", "New Zealand", "Canada", "Netherlands"], "correct": 1},
    {"topic": "Volunteering", "difficulty": "Difficult", "question": "Which of the following is a key principle of the International Red Cross and Red Crescent Movement?", "options": ["Wealth redistribution", "Neutrality", "Political advocacy", "Environmental conservation"], "correct": 1},
    {"topic": "Volunteering", "difficulty": "Difficult", "question": "What is the focus of the United Nations Volunteers (UNV) program?", "options": ["Environmental protection", "Global peace and development", "Educational reform", "Medical research"], "correct": 1},
    {"topic": "Volunteering", "difficulty": "Difficult", "question": "Which legislation in the United States encourages volunteerism and civic engagement?", "options": ["Patriot Act", "Volunteer Protection Act", "Serve America Act", "Civil Rights Act"], "correct": 2},
    {"topic": "Volunteering", "difficulty": "Difficult", "question": "In volunteer management, what does the acronym 'ROI' stand for?", "options": ["Return on Investment", "Rate of Involvement", "Readiness of Individual", "Report of Intent"], "correct": 0},
    {"topic": "Coffee", "difficulty": "Easy", "question": "What is the main ingredient in coffee?", "options": ["Tea leaves", "Coffee beans", "Cocoa powder", "Sugar"], "correct": 1},
    {"topic": "Coffee", "difficulty": "Easy", "question": "Which of the following is a popular coffee beverage?", "options": ["Mojito", "Espresso", "Smoothie", "Lemonade"], "correct": 1}
    {"topic": "Coffee", "difficulty": "Easy", "question": "What does the term 'latte' mean in Italian?", "options": ["Milk", "Coffee", "Cream", "Sugar"], "correct": 1},
    {"topic": "Coffee", "difficulty": "Easy", "question": "Which country is the largest producer of coffee?", "options": ["Vietnam", "Brazil", "Colombia", "Ethiopia"], "correct": 1},
    {"topic": "Coffee", "difficulty": "Easy", "question": "What is a common way to prepare coffee at home?", "options": ["Boiling beans", "Steeping leaves", "Using a coffee maker", "Fermenting grounds"], "correct": 2},
    {"topic": "Coffee", "difficulty": "Moderate", "question": "Which coffee variety is known for its high acidity and floral aroma?", "options": ["Robusta", "Arabica", "Liberica", "Excelsa"], "correct": 1},
    {"topic": "Coffee", "difficulty": "Moderate", "question": "What is the process of removing caffeine from coffee beans called?", "options": ["Fermentation", "Decaffeination", "Distillation", "Extraction"], "correct": 1},
    {"topic": "Coffee", "difficulty": "Moderate", "question": "Which coffee brewing method involves forcing hot water through finely-ground coffee?", "options": ["French press", "Drip brewing", "Espresso", "Cold brew"], "correct": 2},
    {"topic": "Coffee", "difficulty": "Moderate", "question": "What is the term for coffee beans that have been roasted for the longest time?", "options": ["Light roast", "Medium roast", "Dark roast", "Blonde roast"], "correct": 2},
    {"topic": "Coffee", "difficulty": "Moderate", "question": "What is the origin of the coffee plant?", "options": ["South America", "Africa", "Asia", "Europe"], "correct": 1},
    {"topic": "Coffee", "difficulty": "Difficult", "question": "Which component in coffee is primarily responsible for its stimulating effect?", "options": ["Theobromine", "Nicotine", "Caffeine", "Tannin"], "correct": 2},
    {"topic": "Coffee", "difficulty": "Difficult", "question": "What is the name of the traditional Ethiopian coffee ceremony?", "options": ["Jebena Buna", "Tana Qun", "Buna Dabo", "Injera Buna"], "correct": 0},
    {"topic": "Coffee", "difficulty": "Difficult", "question": "What is the term for the thin layer of oils and fine particles on top of a freshly brewed espresso?", "options": ["Froth", "Crema", "Foam", "Scum"], "correct": 1},
    {"topic": "Coffee", "difficulty": "Difficult", "question": "What is 'Kopi Luwak,' and why is it unique?", "options": ["A coffee made from sea salt, popular in Indonesia", "A coffee brewed with volcanic water in Hawaii", "A coffee that includes beans eaten and excreted by civet cats", "A coffee mixed with cocoa powder, popular in Belgium"], "correct": 2},
    {"topic": "Coffee", "difficulty": "Difficult", "question": "What does the term 'terroir' refer to in the context of coffee?", "options": ["The roasting method used", "The flavor profile of the beans", "The growing environment of the coffee plant", "The blending technique of different beans"], "correct": 2},
]

# Scoring System
def calculate_score(difficulty):
    if difficulty == "simple":
        return 1
    elif difficulty == "medium":
        return 2
    elif difficulty == "difficult":
        return 4

# User Interaction
def quiz_session():
    score = 0
    incorrect_answers = []
    questions_session = random.sample(questions, 5)
    for question in questions_session:
        print(f"Topic: {question['topic']}, Difficulty: {question['difficulty']}")
        print(question["question"])
        for i, option in enumerate(question["options"]):
            print(f"{i+1}. {option}")
        user_answer = input("Enter the number of your answer (or 'h' for a hint): ")
        if user_answer.lower() == 'h':
            hint_options = random.sample(question["options"], 2)
            print("Hint: The correct answer is one of the following options:")
            for i, option in enumerate(hint_options):
                print(f"{i+1}. {option}")
            user_answer = input("Enter the number of your answer: ")
            if int(user_answer) - 1 == question["correct"]:
                score += calculate_score(question["difficulty"]) / 2
                print("Correct!")
            else:
                incorrect_answers.append(question)
                print(f"Incorrect. The correct answer is {question['options'][question['correct']]}")
        else:
            if int(user_answer) - 1 == question["correct"]:
                score += calculate_score(question["difficulty"])
                print("Correct!")
            else:
                incorrect_answers.append(question)
                print(f"Incorrect. The correct answer is {question['options'][question['correct']]}")
    print(f"Your final score is {score} out of 10.")
    if incorrect_answers:
        print("You got the following questions incorrect:")
        for question in incorrect_answers:
            print(f"Topic: {question['topic']}, Difficulty: {question['difficulty']}")
            print(question["question"])
            print(f"Correct answer: {question['options'][question['correct']]}")

# Run the quiz session
quiz_session()

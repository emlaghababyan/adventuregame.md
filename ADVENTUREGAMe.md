# establishing commands:
# these commands are to add variables around strings to add aesthetics around stat updates and the title.
#use import time and time.sleep(13) to slow down text
x = "Your relationship with xxxxxxxx has xxcreased!"
title = "Someone's dead?; Strange Things are Happening at Ikebukuro High School"

# title
print("=" * len(title))
print(title)
print("=" * len(title))

# establish relationships with other characters
cass_relationship_stat = 5
joe_relationship_stat = 2
sarv_relationship_stat = 0
UU_relationship_stat = 2

# information that is used for later storylines and desicion making

# commands so that user can use their own pronouns
n = input("Enter your name ")
print("[1] Female")
print("[2] Male")
print("[3] Non-Binary")
pn = input("Select Gender by typing the corresponding number ")
femalepronouns = False
malepronouns = False
nonbinarypronouns = False

# establish pronoun variables
if pn == "1":
    femalepronouns = True

if pn == "2":
    malepronouns = True
if pn == "3":
    nonbinarypronouns = True

# establish the types of pronoun to be used in the game inlcuding some possesive ones.
if femalepronouns == True:
    pronoun1 = "she"
    pronoun2 = "her"
    pronoun3 = "hers"
    pronoun4 = "her"

if malepronouns == True:
    pronoun1 = "he"
    pronoun2 = "him"
    pronoun3 = "his"
    pronoun4 = "his"

if nonbinarypronouns == True:
    pronoun1 = "they"
    pronoun2 = "them"
    pronoun3 = "theirs"
    pronoun4 = "their"

#Introduction to story

print('BRIGHT AND EARLY,' "\n" "thats how everyday started.")
print()

import time
time.sleep(1)
print(
    f"But this morning, something felt odd. In the typically sunny town of Ikebukuro it began to rain, no, storm. The clap of thunder awoke {n} from {pronoun4} sleep."
)

print()

import time
time.sleep(5)

print(
    f'"Holy crap its late," {pronoun1} thought, turning over to check {pronoun4} phone to see what time it was. The phone read 07:53 AM. Somehow, {n} had slept in far beyond {pronoun4} 06:30 alarm.'
)

print()

#  desicion two, wait for friend or dont. This will establish the relationship between player and cassidy and determine her willingness to kill the player

import time
time.sleep(1)
print(
    f"{n} got dressed as quickly as {pronoun1} could and ran out the door. As {pronoun1} speedwalked toward school {pronoun1} heard {pronoun4} childhood friend, Cassidy, from down the road."
)

print()

import time
time.sleep(5)
print(f'"Hey, {n}! Wait up!"')

print()

import time
time.sleep(2)
print(
    f"{n} stops in {pronoun4} track. Knowing that by stopping and waiting {pronoun1} will surely be late."
)

print()
import time
time.sleep(3)
print('"Looks like Cassidy wants to catch up to me."')

print("[1] Stay and wait. Being on time is for nerds anyways.")
print("[2] Every man for themselves! It's not my fault she woke up late.")

print()
# some choices alter the relationship between the user and the characters.
# choice 2 alters the relatioship between user and cass
choice2 = input("CHOICE ")
if choice2 == "1":
    cass_relationship_stat = cass_relationship_stat + 1
    print()
    import time
    time.sleep(1)
    print(
        '"You know what. School can wait, my friends are more important than morning announcements."'
    )
    import time
    time.sleep(4)
    print(
        f'{n} sighs and stands still in the pouring rain for a few seconds waiting for Cassidy to jog up to {pronoun2}. "Took you long enough," {n} scoffed, crossing {pronoun4} arms.'
    )

    print()

    import time
    time.sleep(4)
    print(
        f'"It was only a few seconds! Come on, we are going to be late for class." Cassidy playfully hit her friend on the shoulder and began to run to school. {n} groaned and lazily jogged along.'
    )
    print()
    import time
    time.sleep(6)

    print(
        "When the two of them arrived at school just a few minutes late, the teacher shot them a dirty look. The pair didn't care so much and laughed to eachother as they sat in their respective seats."
    )
    import time
    time.sleep(6)

    print()

    print("Your relationship with Cassidy has increased!")
    print("=" * len(x))
    import time
    time.sleep(7)

if choice2 == "2":
    cass_relationship_stat = cass_relationship_stat - 2
    print()
    print("I really should hurry up, I'll be late")
    print()
    import time
    time.sleep(1)
    print(
        f'Even though {pronoun1} probably made the smarter desicion by walking alone, {pronoun1} still showed up to class late with a very upset teacher. With a bitter face she instructed {n} to take {pronoun4} seat, repeating the same thing only a few minutes later to Cassidy, who shot a glare at {n} as she sat down.'
    )
    import time
    time.sleep(7)

    print("=" * len(x))
    print("Your relationship with Cassidy has decreased!")
    print("=" * len(x))
    import time
    time.sleep(7)

import time
time.sleep(2)

print(
    f'"Alright, I hope you guys studied well for our math test today." A math test?! Seriously? Just how unlucky could today get?'
)
print()
import time
time.sleep(10)
import time
time.sleep(8)
print(
    f"The teacher placed the test on {n}'s desk. {pronoun1} groaned. {pronoun1} obviously knew very little about the subject matter presented to {pronoun2}, although there were a solid few questions {pronoun1} could answer a question or two confidently. {n} decided to waste the rest of the period looking around the classroom to find something to entertain {pronoun2}"
)
import time
time.sleep(8)
print()
print(
    f"{n}'s eyes fell upon one of {pronoun4} classmates, Sarvnaz, who {n} had a crush on since elementary school. She was clearly struggling on a question that {n} had actually been able to solve. {pronoun1} could help out but {pronoun1} doesn't want to come off TOO strong and doesn't want the teacher to catch {pronoun2}."
)
print()
import time
time.sleep(1)
print("Help Sarvnaz out?")
print()
print("[1] Yeah sure. It's not like I'll pass this test anyways.")
print("[2] No way. Then she'll totally know I have a crush on her.")
choice3 = input("CHOICE ")
# CHOICE THAT DETERMINES GAME OUTCOME
if choice3 == "1":
    import time
    time.sleep(2)
    print(
        f" {n} loudly sighs to get Sarvnaz's attention. She looks in {pronoun4} direction and notices that the test is shifted towards her. A slight smile rises on her face as she quickly copies down the work {n} has done onto her own paper,adjusting it a bit so that it does not look exactly the same."
    )
    import time
    time.sleep(8)
    sarv_relationship_stat += 3
    print()
    print("=" * len(x))
    print("Your relationship with Sarvnaz has increased!")
    print("=" * len(x))
    import time
    time.sleep(7)

if choice3 == "2":
    import time
    time.sleep(2)
    print(
        f"{n} continues on {pronoun4} hunt for the most distracitng item in the room when all of a sudden, {pronoun1} makes direct eye contact with Sarvnaz. {n} can tell she's practically begging for a helping hand, but {n} decided to ignore her."
    )
    import time
    time.sleep(8)
    sarv_relationship_stat -= 3
    print("=" * len(x))
    print("Your relationship with Sarvnaz has decreased!")
    print("=" * len(x))
    import time
    time.sleep(7)

import time
time.sleep(1)
print()
print(
    f"All of a sudden, in the middle of the test, the loudest sound of thunder {n} had ever heard in {pronoun2} life. The lights in the school began to flicker and the teacher told the class to stay calm."
)
print()
import time
time.sleep(6)
print(
    f'"Alright don\'t worry. The emergency lights will turn on any minute now." The entire class sat in total darkness for 15 minutes in the pitch black. {n} could hear the sound of the children in the lower grades screaming and crying, presumably because of the darkness and the loud thunder.'
)
print()
import time
time.sleep(10)
print()
print(
    "All of a sudden the winds outside get harsher and harsher and the windows shattered open. This is when a lot of the older kids began to freak out, as a few had been injured greatly by the flying glass."
)

import time
time.sleep(4)

print(
    f"{n} sees two of {pronoun4} friends lying down on opposite ends of the room. One of them is harshly impaled on their leg, and the other is experiencing an anxiety attack."
)
import time
time.sleep(2)
print()
print(
    f"The friend with the injury, Joe, has many friends surrounding him, but {n} took first aid courses because of {pronoun4} volunteer program requirements. On the other hand, You You, the other friend, was totally alone, but {n} had no clue how to handle someone with a panic attack. Who do you try to help?"
)
import time
time.sleep(8)
print()
print("[1] Help Joe")
print("[2] Help You you")
choice4 = input("CHOICE ")
if choice4 == "1":
    print(
        '"My time is better spent helping someone who I know I can surely help"'
    )
    print()
    import time
    time.sleep(3)
    print(
        f"{n} quickly sat up and crawled over to where Joe was stationed. {n}'s classmates moved aside so that {pronoun1} could handle the situation. It appeared that there had been a large glass shard inside his leg, so {n} took {pronoun4} school blazer and wrapped it around the space above the leg to stop blood flow to the wound."
    )
    import time
    time.sleep(8)
    joe_relationship_stat += 4
    UU_relationship_stat -= 6
    print("=" * len(x))
    print("Your relationship with Joe has increased!")
    print("Your relationship with You You has increased!")
    print("=" * len(x))
if choice4 == "2":
    print(
        f'Although {n} has little knowledge on how to calm down someone in an episode, {n} graps You You\'s hands and looks her in the eyes. "Lets count to ten, Okay?" You You not understanding at first allows {n} to take lead. She then understands what is going on and counts along. The two continue to count until You You breathes steadily and stops crying.'
    )
    import time
    time.sleep(4)
    joe_relationship_stat -= 3
    UU_relationship_stat += 7
    print("=" * len(x))
    print("Your relationship with You You has increased!")
    print("Your relationship with Joe has decreased!")
    print("=" * len(x))
    print(
        f"{n} looks at the bandaging on Joe's leg knowing that {pronoun1} could have done better."
    )
print(
    f"After helping {pronoun3} friend, {n} crawled back to safety with the rest of the class."
)
import time
time.sleep(3)
print()
print(
    '"This is getting ridiculous" the teacher frantically panics, trying to keep Joe calm about his injury. "I have no connection to the administration." She looks at the door. "Kids, I will be right back. Stay in this corner and make sure his wound does get infected" she points to Joe and to the first aid kit on the wall.'
)
print()
import time
time.sleep(8)
print(
    "The teacher hurried out of the room and down to the office. All had been fine until we heard a gutteral scream come from the lower floor."
)
print()
import time
time.sleep(6)
print(
    f'"Oh my god what was that??" You You panics. {n} reassures her and says that {pronoun1} will go check it out.'
)
print()
import time
time.sleep(5)
# try and make a version where user gets to select which character to go with

print(
    f'"Sarvnaz will you come with me?" {n} asks, but when {pronoun1} looks around the room, Sarvnaz is nowhere to be seen. "Oh, uh then Cassidy can you come along?"'
)
print()
import time
time.sleep(7)
print(
    'She nods and gets up from where she was sitting. The two students leave the classroom into the pitch black hallway. Cassidy uses the flashlight on her phone to illuminate the hallway.'
)

print()
print(
    'The two go down a set of stair and reach the first floor.The entire floor is empty. No classrooms, no doors, except for the end of the hall; a door that laid ajar. They slowly made their way towards the door when all of a sudden the ground beneath Cassidy collapses into the basement of the school.'
)

print()

import time
time.sleep(12)
print(
    f'"Oh my god! Oh my god oh my god help!!" Cassidy shouts as she slips through the crack. Her single hand holds herself up from the edge of the hole. {n} does not know if {pronoun1}  can lift her back up alone, but if {pronoun1} tries to go get help she may fall before {pronoun1} gets back.'
)

print()

print("[1] Help her by myself! Quickly!")
print("[2] Run back to class and get help. There's no way I can pick her up")
choice5 = input("CHOICE ")
if choice5 == "1":
    print(
        f"{n} kneels onto the hardwood floor and  reaches down to grab her hand that was not gripping the surface."
    )
    import time
    time.sleep(7)

    print(
        f"All of a sudden the ground below {n} began to break, so {pronoun1} quickly got up from the ground and the wood beneath {pronoun2} broke. In what appeared to be just seconds, Cassidy fell 15 feet under the ground. {n} screamed and shouted into the hole."
    )
    import time
    time.sleep(9)

    print()

    print(
        f'"CASSIDY! ARE YOU OKAY?" there was no response. {n} fell on {pronoun2} bottom, {pronoun4} hands shakingly covering their mouth. Slowly tears began falling down {pronoun4} face.'
    )

    print('"CASSIDY!" There was still no response.')
    import time
    time.sleep(7)
if choice5 == "2":
    print()
    print(
        f'{n} kneeled down to where Cassidy hung "Hold on, I need to go get help!"'
    )
    import time
    time.sleep(3)
    print()
    print(
        f"Cassidy screamed in retaliation. As {n} stood up from the the ground beneath {pronoun2} began to crack, and without thinking, {n} jumped off. The chunk of the floor, along with Cassidy herself."
    )
    import time
    time.sleep(8)
    print()
    print(
        f'"CASSIDY! ARE YOU OKAY?" there was no response. {n} fell on their bottom, {pronoun4} hands shakingly covering their mouth. Slowly tears began falling down {pronoun3} face. "CASSIDY!" There was still no response.'
    )
    import time
    time.sleep(11)
print(
    f"{n} felt a stir in {pronoun3} stomach as {pronoun1} just realized {pronoun1} was probably the reason {pronoun4} friend was dead"
)
import time
time.sleep(11)
print()
print(
    f'"Oh god I have to go tell the others" {n} thought, feeling the familiar queasy feeling in {pronoun4} stomach again. How could someone explain something like this?'
)
import time
time.sleep(8)
print()
print(
    f"All of a sudden, {n} remembered the reason the two of them went down to the first floor; to find their teacher. What if something bad happened to her? Things weren't normal here. No, it's like the school is haunted or something. Like it's trying to kill us."
)
import time
time.sleep(11)
print("Do I go and tell the others or try and see if I can find our teacher?")
print()
print("[1] Go back upstairs and warn the others!")
print("[2] Go and see if I can save our teacher before it's too late.")
choice6 = input("CHOICE ")
if choice6 == "2":
    print(
        f'{n} calmed down and took a deep breath. Before {pronoun1} could stand up properly {pronoun1} heard a call of {pronoun4} name.'
    )
    print()
    import time
    time.sleep(6)
    print(
        f'{n} turned around to look at the source of the noise, and discovered You You peaking her head through the staircase doorway. "Huh? What happened here?! Where\'s Cassidy?" {n} nervously shuffled and with a shaky voice explained how Cassidy fell into the hole.'
    )
    import time
    time.sleep(9)
    print(
        f'"No... there\'s no way that happened! That fall is so deep, if she fell then there\'s no way..." You You went silent "Yeah.. I think so too.."{n} said, tears swelling in {pronoun4} eyes'
    )
    print()
    import time
    time.sleep(6)
if choice6 == "1":
    print(
        f"{n} turns around and heads straight for {pronoun4} classroom, walking extremely slowly and listening out for any creaks of wood from under {pronoun4} feet."
    )
    print()
    import time
    time.sleep(11)
    print(
        f'When {n} got to the door, {pronoun1} realized that {pronoun1} had no clue what to tell the class. Cassidy died because of my stupidity? Slowly, {n} opened the door of the classroom, and all attention was shifted onto {pronoun2}'
    )
    print()
    import time
    time.sleep(11)
    print(
        '"Hey guys..." all of a sudden, {n} was bombarded with questions, but the most pressing issue was where Cassidy was. "Really, there is no way I can explain it to you guys... but this storm is doing really, really weird things to this school. I can\'t go much further than that, but I need you all to stick together while I investigate-" all of a sudden, You You interupted {n}\'s speech, \n "I want to come with you!"'
    )
    import time
    time.sleep(11)
    print('"You You, I don\'t know if thats such a good idea.."')
    import time
    time.sleep(2)
    print()
    print('"No! I want to help!" You You protested.')
    print()
print("Should I let You You come?")
print("[1] Let her come. We're safer in groups")
print("[2] No way. She'll just slow me down.")
choice7 = input("CHOICE ")
if choice7 == "1":
    import time
    time.sleep(2)
    print(
        '"Alright you can come along. But be careful. There\'s no telling which one of us will get injured next"'
    )
    import time
    time.sleep(2)

if choice7 == "2":
    print('"No way. It\'s too dangerous" {n} says sternly')
    print()
    import time
    time.sleep(2)
    print(
        '"I\'m afraid you\'ve misunderstood me, {n}. I was not asking. I\'m coming whether you like it or not." You You says, with a stronger energy than {n} had ever seen from her before.'
    )
    import time
    time.sleep(5)
    print("=" * len(x))
    UU_relationship_stat -= 3
    print("Your relationship with You You has decreased!")
    print("=" * len(x))

print(f'"Did you find Ms. Fujiosha?"')
print()
import time
time.sleep(2)
print(
    f'"No, we were going to go into that door..." {n}pointed to the direction of the door that was slightly ajar, but when {pronoun1} looked in the direction, there was no longer a door.'
)
import time
time.sleep(5)
print(
    f"{n} ran up to where the door was supposed to be, gliding {pronoun4} hands along where the frame should have been."
)
import time
time.sleep(4)
print(
    f'"No! There\'s no way.. I swear there was a door there before!" {n} kicks the wall in frustration and out of nowhere a door appears and creaks open. {n} falls backwards onto the ground in fear and points at the door. You You gasps and walks towards it slightly, hesitantly reaching forward to push it open.'
)
print()
import time
time.sleep(10)
print(
    'You You lets out a whimper as her eyes behold the site in front of her. A large, demonic dog resembling Cerberus laid towering over the deceased body of their teacher. At the sound of You You\'s whimper the beast looks up at the door and opens it\'s eyes wide. The flesh of the eye is solely white. It appears to have some sort of cataract and clearly cannot see the two students standing behind the door. It lower\'s its gaze and continues to eat.'
)
import time
time.sleep(15)
print("You You shuts the door closed as fast as she can and begins to cry.")
print(
    '"I can\'t do this.. I can\'t do this." she cries over and over again into her palms."'
)
print()
import time
time.sleep(2)
print(
    f"{n} stands still pitying the girl who sobbed in front of {pronoun2}. None of this was normal. None of this should be happening. This isn't Ikebukuro High. This is more like hell."
)
print()
import time
time.sleep(7)
print(
    f'"When you went in there, what did you see?" {n} asks, looking You You in her quivering eyes'
)
import time
time.sleep(2)
print(
    '"It was the gym. The gym I think. It had a huge door in the back." she stuttered, wiping the tears from her cheeks.'
)
print()
import time
time.sleep(4)
print(
    f'"The door at the back of the gym.. The door that has a giant exit sign on it?" {n} shook You You\'s shoulders quickly. This could be their way out!'
)
print()
import time
time.sleep(10)
print('"Yeah, that\'s the one"')
print()
print(
    f'"Okay, this could be our way out. But first, we need to go upstairs to get the others." {n} explains.'
)
print()
import time
time.sleep(4)
print(
    "The two quickly trudge upstairs and back to their classroom, very wary of the decaying floor beneath them. Eventually they reach their classroom again."
)
print()
import time
time.sleep(4)
print(
    "When You you opens the door, there's only one person sitting in the room. Joe, weak and injured."
)
print()
print(
    f'"Oh my god! There\'s something wrong with him! get me the first aid kit!" {n} instructs You You. She nods and quickly removes the small white box off of the wall. Quickly, {n} opens it and looks through the material. {pronoun1} take a pad of alcohol and uses it\'s strong scent to knock Joe back into consciousness.'
)
import time
time.sleep(8)
print()
print(
    f'Slowly, Joe wakes up from his slumber. "Huh? What\'s going on?!" he shouts, confused.'
)
import time
time.sleep(3)
print()
print(
    '"Hey, calm down," You You shushes. "We need to get you out of here. Where is everyone else?" she asks frantically."'
)
import time
time.sleep(6)
print()
print(
    f'"They all left one by one.. they said they would come back but none of them have." You You chokes up, about to cry. "Hey, where\'s Cassidy? wasn\'t she with you, {n}?"'
)
print()
import time
time.sleep(6)
print(
    '"We\'ll talk about Cassidy later. right now, we\'ve got to get you out of here. Can you walk?"'
)
print()
import time
time.sleep(4)
print('"No.. my leg is numb from the thigh down." He points to the leg wound.')
print()
import time
time.sleep(2)
print('"I could try and pick him up and carry him on my back?"')
import time
time.sleep(2)
print(
    f'"That could work," You You muttered. She tried to help joe stand up from his sitting position and onto {n} back.'
)
import time
time.sleep(4)
print()
print(
    'The group heads back down the stairs slowly, being sure as to not further worsen Joe\'s injury.'
)
import time
time.sleep(5)
print(
    f"{n}, Joe and You You all make it back down to the stairs safe an intact, for now."
)
print()
import time
time.sleep(4)
print(
    f'"Okay, how are we going to go about doing this? one by one?" You You begins, but then realizes that {n} had a person clinging onto them for dear life.'
)
import time
time.sleep(7)
print()
print('"One of us needs to go first, but one of us needs to carry Joe."')
import time
time.sleep(4)

print("[1] I can carry Joe, You You needs to go first")
print("[2] You You should carry Joe so that I will go first.")
choice8 = input("CHOICE ")
if choice8 == "1":
    import time
    time.sleep(2)
    print('"I\'ll carry Joe in. You go first."')
    print()
    import time
    time.sleep(2)
    print(
        f"You You nods as she takes a deep breath and opens the door. The dog is staring directly towards us, but it doesn\'t seem to see us. {n} adjusts Joe on {pronoun4} back and walks in. Things go smoothly at first, that is, until the shoes on {n} feet make a loud squeaking sound on the waxed floors of the gymnasium.'"
    )
    import time
    time.sleep(18)
    print(
        f"The dog looks directly at {n} and lungles forward. {n} screams as Joe is ripped off of {pronoun4} back and eats him in one foul swoop. {n} sprints as fast as {pronoun4} could,and ran towards the exit with You You."
    )
    import time
    time.sleep(13)

if choice8 == "2":
    import time
    time.sleep(2)
    print('"I\'ll carry Joe in. You go first." You You said, determined.')
    print()
    import time
    time.sleep(2)
    print(
        f"You You nods as she takes a deep breath and opens the door. The dog is staring directly towards us, but it doesn\'t seem to see us. You You adjusts Joe on her back and walks in. Things go smoothly at first, that is, until the shoes on You You feet make a loud squeaking sound on the waxed floors of the gymnasium.'"
    )
    import time
    time.sleep(18)
    print(
        f"The dog looks directly at You You and lungles forward. {n} screams as Joe is ripped off of her back and eats him in one foul swoop. Because of her flight or fight response, You You sprints as fast as she could,and ran towards the exit with {n}."
    )
    import time
    time.sleep(13)
print(
    'The twp students pant and wheeze, realizing what had happened as the blood of their friend was stained on their white uniforms. You You again starts to cry as she realizes how many people she cared about she had lost in one day.'
)
import time
time.sleep(15)
print(
    '"Well well well. I didn\'t think the two of you had it in you to survive"'
)
print()
print(
    f"It wasn't until now did {n} realize exactly where they were, or to put it simply where they werem't. A purple void surrounded them, seeming almost ethereal. Looking up, {n} saw Sarvnaz smiling at them."
)
import time
time.sleep(13)

print('"Sarvnaz?" You You beckons. "Is that you?"')
print()
import time
time.sleep(2)
print(
    '"Of course, stupid. No, I\'m actually the queen of England." she snickers into her hand.'
)
print()
import time
time.sleep(4)
print(
    f'"Wait what?! Is this some sort of prank? Did you drug us or something?"{n} asked, panic evident in {pronoun4} voice'
)
print()
import time
time.sleep(13)
print(
    '"Oh god no. This is all real! every last bit of it. You see, I\'m not actually some cute schoolgirl you\'ve had a crush on since you were a kid. I\'m actually a demon who feasts on the souls of kids! But now that I think about it, I\'m not that far from a regular teenage girl." She laughs maniacally at her own joke.'
)
print()
print(
    f'"I guess you deserve a reward for making it out here alive." She mutters, circling the two teenagers.'
)
if sarv_relationship_stat > 0:
    print(
        f'"Okay {n}! Since you were extra nice to me during the test today, I\'ll let you choose who wins or dies!"" she laughs again. Like it\'s some sort of sick game for her.'
    )
    print()
    import time
    time.sleep(13)
    print(
        '"So. Who will you choose? Who gets to live, and remember, the other gets sent straight to hell!"'
    )
    print("[1] Me.")
    print("[2] You You.")
    choice9 = input("CHOICE ")
    if choice9 == "1":
        print(
            '"Wow! thats pretty heartless huh. Well then, You You, I hope you brought your tanning lotion! It gets pretty hot down there!"'
        )
        print(
            f"All of a sudden everything fades to black. Actually, {n} can't remember where I was just now.. or what {pronoun1} was doing..."
        )
        import time
    time.sleep(13)
    print("END")
    if choice9 == "2":
        print(
            '"Aww how chivalrous! If I wasn\'t totally starving I might actually consider sparing the two of you! Oh well." She smiles and then whisks You You away. "Oh Yum! I love dessert!"'
        )
        import time
        time.sleep(13)
        print("END")
else:
    print(
        '"Oh but I haven\'t eaten in so so long... I guess I could just pig out and not spare either of you! Sounds delicious! Hope you guys brought sunscreen, it gets hot down there in hell!" The last thing You you or {n} ever hears is the teenage girl\'s maniacal laughter as their souls are slowly drained from their bodies.'
    )
    print("END")

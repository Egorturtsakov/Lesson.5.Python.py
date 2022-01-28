# Lesson.5.Python.py

Номер 1:

import random
 
def getRandomOdd(start = 0, end = 10):
    
    return random.randrange(start // 2, end // 2) * 2 + 1
 

def main():
    
    for i in range(100):
        
        print(getRandomOdd())
 

if __name__ == "__main__":
    main()
    
    
Номер 3:

tutors = [
    'Иван', 'Анастасия', 'Петр', 'Сергей',
    'Дмитрий', 'Борис', 'Елена'
]


klasses = [
    '9А', '7В', '9Б', '9В', '8Б', '10А', '10Б', '9А'
]


def gen_of_people():

    i = 0
    
    j = 0
    
    while i < len(klasses)
    
        if i >= len(tutors)
        
              yield (None, klasses[i])
              
              i += 1
              
              j += 1
              
              break
              
        else:
        
            yield (tutors[j], klasses[i])
            
            i += 1
            
            j += 1
            
    

for gen in gen_of_people():

    print(gen)
    

  
  Номер 5:
  
  lst = [1, 2, 4, 5, 6, 2, 5, 2]

used = set()

unique = [x for x in lst if x not in used and (used.add(x) or True)]

print(unique)


from collections import Counter

counter = Counter(lst)


unique = list(counter)

print(unique)


single = [x for x,n in counter.items() if n==1]

print(single)

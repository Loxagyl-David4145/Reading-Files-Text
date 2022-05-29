# Reading-Files-Text
Texts Count and number outputs

#openfile = open("./story.txt", "r")
def readfile(filename):
    #reading the files
    with open("C:/Users/user pc/Source/repos/100DaysOfCode/Reading-Text-Files/story.txt", "r") as openfile:
        read_file = openfile.read()
    return read_file


def count_words():
    text = readfile("C:/Users/user pc/Source/repos/100DaysOfCode/Reading-Text-Files/story.txt")
    split_text = text.split()
#print(split_text)
    count = {}
    for i in split_text:
        if i in count:
            count[i] += 1
        else:
            count[i] = 1
    return count


print(count_words())

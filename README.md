# Week4__reverselist
#Allen Simmons

"""
Given a Linked List which represents a sentence S such that each node
represents a letter, the task is to reverse the sentence without reversing
individual words.
  - Ex.)
  Input:  I-> ->l->o->v->e-> ->G->e->e->k->s-> ->f->o->r-> ->G->e->e->k->s->NULL
  Output: G->e->e->k->s-> ->f->o->r-> ->G->e->e->k->s-> ->l->o->v->e-> ->I->NULL
"""

def reverse(S):
    list1 = ""
    length = len(S) - 1
   # print(length)
    for position in range(length, -1,-1):
        #print(position)
        list1 =  list1 +  S[position]
        #print(list)

    return list1

S = [" I ", " love ", " Geeks ", " for ", " Geeks "]
#my code doesn't use stacks or queues, it reads the length of 6 -1 = 5.
#set list1 equal to list1 + the item in the index position, looped.

print(reverse(S))

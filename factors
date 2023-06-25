#!/usr/bin/python3
""" My module for testing numbers and finding the factorization """
import math
from sys import argv


def factor(number, test_num):
    """ Finds the values to return once a number has been found
    """


    print("{}={}*{}".format(number, (number // test_num), test_num))


with open(argv[1], mode="r", encoding="UTF-8") as f:
    for line in f:
        number = int(line)
        if number % 2 == 0:
            factor(number, 2)
        else:
            max_number_to_test = math.floor(math.sqrt(number))
            for test_num in range(3, max_number_to_test + 1, 2):
                if number % test_num == 0:
                    factor(number, test_num)
                    break
                            


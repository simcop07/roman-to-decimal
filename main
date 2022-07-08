numbers = {
    "I": 1,
    "V": 5,
    "X": 10,
    "L": 50,
    "C": 100,
    "D": 500,
    "M": 1000
}

def check_chars(roman):
    for c in roman:
        if c not in numbers:
            return False
    return True

def RtD(roman):
    if not check_chars(roman):
        return -1
    roman = roman.upper()
    dec = 0
    for i, d in enumerate(roman[:-1]):
        if numbers[d] < numbers[roman[i + 1]]:
            dec -= numbers[d]
        else:
            dec += numbers[d]
    dec += numbers[roman[-1]]
    return dec

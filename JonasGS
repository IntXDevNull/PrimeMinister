import itertools

# Passwords will be generated based on the worn out keys on the keyboard from his picture.
keys = ['E', 'R', 'T', 'A', 'S', 'D', 'F', 'Ø', 'Å']

# Password length settings. Example below: 4 to 6 characters which is typical windows hello length.
min_length = 4
max_length = 6

output_file = "password_list.txt"

def generate_passwords():
    with open(output_file, 'w') as file:
        for length in range(min_length, max_length + 1):
            for combination in itertools.product(keys, repeat=length):
                password = ''.join(combination)
                file.write(password + '\n')
                print(f"Generated: {password}")

def main():
    print("Starting password generation...")
    generate_passwords()
    print(f"Password list saved to: {output_file}")

if __name__ == "__main__":
    main()

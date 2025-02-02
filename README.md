def count_words(text):
    """Function to count the number of words in the given text."""
    words = text.split()
    return len(words)

def main():
    """Main function to handle user input and display word count."""
    print("Welcome to the Word Counter Program!")
    
    # Get user input
    text = input("Enter a sentence or paragraph: ").strip()

    # Error handling for empty input
    if not text:
        print("Error: No input provided. Please enter some text.")
        return

    # Count words
    word_count = count_words(text)

    # Display output
    print(f"Word Count: {word_count}")

if __name__ == "__main__":
    main()


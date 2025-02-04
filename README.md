<<<<<<< HEAD
# nlp-a1
=======
# Shakespearean Text Generator 📜

Welcome to my NLP assignment for the **AI: Natural Language Processing & Semantic Analysis** course at IE University. This project is all about generating text that sounds like William Shakespeare using **N-gram models** with Python and NLTK.

---

## 🚀 What I Did

1. **Data Preparation:**  
   - Loaded *Much Ado About Nothing* text.
   - Preprocessed it: converted to lowercase, removed punctuation, and tokenized the text using NLTK.

2. **Bigram, Trigram, and Quadgram Models:**  
   - Created bigrams (2-grams), trigrams (3-grams), and quadgrams (4-grams) using NLTK's `ngrams` function.
   - Counted how often each word follows these N-grams.

3. **Probability Distribution:**  
   - Calculated the probability of the next word appearing after each N-gram.
   - Used basic probability calculation without any smoothing or temperature scaling.

4. **Sampling Next Token:**  
   - Implemented a function to sample the next word based on these probabilities.
   - Used **weighted random choice** for selecting the next token.

5. **Generating Text:**  
   - Built functions to generate text starting from an initial phrase.
   - Added a **fallback system**: if quadgram doesn’t work, it falls back to trigram, then bigram, then random word.

6. **Experimentation:**  
   - Tested with different starting phrases.
   - Analyzed how bigrams, trigrams, and quadgrams affect text quality (quadgrams are more coherent, bigrams are more random).

---

## 💻 How to Run It

1. Install required libraries:
   ```bash
   pip install nltk
   ```

2. Run the notebook `nlp_assignment1.ipynb`.

3. To generate text:
   ```python
   start_ngram = ('i', 'am', 'of')  # Starting phrase
   generated_text = generate_text_with_fallback(start_ngram, 100, [from_quadgram_to_next_token_probs, from_trigram_to_next_token_probs, from_bigram_to_next_token_probs])
   print(generated_text)
   ```

---

## 🎯 Key Takeaways

- **Bigrams** = Random, fun, but less coherent.
- **Trigrams** = A nice balance of coherence and creativity.
- **Quadgrams** = Makes more sense, feels like real Shakespeare!

Hope you enjoy the Bard vibes! 🤓✨
>>>>>>> ca50578 (Initial commit)

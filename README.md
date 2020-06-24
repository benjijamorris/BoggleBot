While playing Boggle online with my family during quarantine, we were joined by a superhuman boggle player. Inspired, I set out to create a Boggle Bot of my own. Using a small number of training images, edge detection, and image augmentation, I trained a Convolutional Neural Network to achieve 98+% accuracy on a small test set to identify Boggle boards from a screenshot of the online boggle site. To identify all words in the boggle board, word prefixes are stored as a 4-tuple containing the x and y coordinates of a letter, a prefix ending at that position, and a list of the positions of letters used to spell that word. To prevent expanding prefixes that don't lead to any words, a trie is created from a version of the SCOWL dictionary to check prefixes quickly. In the future, I hope to makethe CNN more robust to pictures of boggle boards not coming from website screenshots. This project is intended to be run on Google Colab.

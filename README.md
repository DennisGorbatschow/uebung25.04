# uebung25.04
void main() {
  List<String> words = ['Wort', 'auge', 'Apfe'];
  List<String> newList = getNewList(words);
  print(newList);
}

List<String> getNewList(List<String> words) {
  List<String> better = [];
  for (int i = 0; i < words.length; i++) {
    if (words[i].length < 5 && words[i].toLowerCase()[0] == 'a') {
      better.add(words[i]);
    }
  }
  return better;
}

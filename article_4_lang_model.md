# Language Model

## 1 Storing Data
* Consider a data set of words

        'one', 'two', 'three', 'four', 'five'

* The first step, is to join the words together
* But a delimeter such as a full stop '.' is required so we know the words are split

        one.two.three.four.five

 ## 2 Construct Neural Network
 * A strategy to convert the data into a neural network is to **predict a word based on three existing words in the dataset** 
 
 ### 2.1 Layers:
 ---
Three layers can be implemented. The idea is to make sure each word is assessed using the context of the previous word. This functionality of each layer is summarised in the following table: 

<!--- Table Explaining Concepts--->
| Layer Level | Function|
| :---        |     :---      |
| `First`  | Only uses the first word as input. It is the embedded layer, that translates input word to hidden word.|
| `Second` | Embedded by second word and uses output of first layer. Provides connection from hidden datapoint to another hidden datapoint.  |
| `Third` | Embedded by third word and uses output of second layer. Outputs the fourth word with an associated probability.  |

Another important feature of the algorithm is the implementation of a **universal weight matrix** for all three layers. This ensures the **same three words arranged differently yields the same predicted word**. 






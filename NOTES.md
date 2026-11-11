classification is a predictive modeling technique where an algorithm assigns input data into predefined categories based on patterns it has learned from training examples.



PS C:\\Users\\slima\\git-lab> python .\\main.py

DEBUG: loaded 36 flows, first rows: \[{'flow\_id': '1', 'src\_ip': '10.0.0.28', 'dst\_ip': '192.168.1.2', 'dst\_port': '80', 'bytes': '997405', 'packets': '7995', 'duration\_s': '3.33', 'label': 'attack', 'attack\_type': 'DoS', 'attack\_prob': 0.5}, {'flow\_id': '2', 'src\_ip': '10.0.1.139', 'dst\_ip': '192.168.1.8', 'dst\_port': '443', 'bytes': '179835', 'packets': '81', 'duration\_s': '56.0', 'label': 'normal', 'attack\_type': 'none', 'attack\_prob': 0.15}]

IDS evaluation report (decision threshold = 0.40)

Flows: 36  (attacks: 14, normal: 22)



&#x20;                 pred. attack  pred. normal

actual attack               12             2

actual normal                4            18



Precision: 0.75

Recall:    0.86

F1 score:  0.80

Most missed attack type: DoS (0 missed)


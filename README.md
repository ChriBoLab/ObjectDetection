# Object Detection
Object detection using cv2.matchTemplate and custom template matching algorithm


## Introduction

### cv2.matchTemplate
Η εικόνα η οποία έχουμε στην διάθεση μας είναι η παρακάτω.

<p align="center">
<img width="50%" src="Input/PythonPitStop.jpg" />
</p>

Στόχος μας είναι να εφαρμόσουμε τεχνικές sliding window  ώστε να εντοπίσουμε από την εικόνα τo σημείo που βρίσκεται το σύμβολο της Python.


<p align="center">
<img width="20%" src="Input/Pythonsymbol.png" />
</p>

Για να δούμε πως εξελίσσεται ο  αλγόριθμος εντοπισμού σε συνθήκες θορύβου θα τον εφαρμόζουμε σε εικόνες στις οποίες έχουμε προσθέσει 5%, 10% και 20% θόρυβο αντίστοιχα.


### custom template matching algorithm
Αφού  πειραματιστήκαμε με τον παραπάνω αλγόριθμο ήρθε η στιγμή να υλοποιήσουμε τον δικό μας αλγόριθμο. Εφαρμόζοντας ένα sliding window στην εικόνα η οποία είναι προς αναζήτηση. Για κάθε παράθυρο που παίρνουμε θα συγκρίνουμε τα ιστογράμματα του παραθύρου και του template το οποίο ψάχνουμε, θα ορίσουμε ένα threshold το οποίο θα ορίζει ποτέ θα θεωρούμε ότι έχουμε matching.

Οι δυο μέθοδοι σύγκρισης που θα χρησιμοποιήσουμε είναι: **Correletion**, **Intersection** .

Αυτήν την φορά θέλουμε να βρούμε το σύμβολο της python το οποίο είναι πίσω από τον οδηγό.

<p align="center">
<img width="20%" src="Input/Python_symbol2.png" />
</p>

## Results

<p align="center">
<img width="90%" src="Input/Detected_orreletion.jpg" />
<br>
Figure 1. <b>Correletion</b> 
</p>

<p align="center">
<img width="90%" src="Input/Intersection.jpg" />
<br>
Figure 2. <b>Intersection</b> 
</p>


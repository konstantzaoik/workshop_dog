# Δημιουργήστε ένα μοντέλο μηχανικής μάθησης

## Περίληψη

Το Azure [Custom Vision](https://docs.microsoft.com/azure/cognitive-services/custom-vision-service/?WT.mc_id=academic-49102-chrhar) σας δίνει τη δυνατότητα να δημιουργήσετε μοντέλα για κατηγοριοποίηση και ανίχνευση αντικειμένων σε εικόνες. Αυτά μπορείτε να τα χρησιμοποιήσετε για να αναγνωρίσετε τη ράτσα ενός σκύλου, εάν κάποιος φοράει κράνος, ή την παρουσία άλλων χαρακτηριστικών. Αν και αυτό μπορεί να γίνει γράφοντας κώδικα και με τη χειροκίνητη επεξεργασία των εικόνων, το Custom Vision παρέχει μία web-based υλοποίηση και εργαλεία για διευκόλυνση της διαδικασίας. Δεν απαιτείται καμία προηγούμενη γνώση μαθηματικών ή μηχανικής μάθησης!

Κατά την διάρκεια αυτού του εργαστηρίου θα δημιουργήσετε ένα μοντέλο για την ανίχνευση της ράτσας σκύλων. Θα ξεκινήσετε με την εγκατάσταση και παραμετροποίηση των απαραίτητων εργαλείων, έπειτα θα δημιουργήσετε το προσαρμοσένο μοντέλο ανεβάζοντας εικόνες και βάζοντάς τους ετικέτες, και τέλος θα χρησιμοποιήσετε το μοντέλο με ένα Κιτ Ανάπτυξης Λογισμικού (SDK).

| **Στόχος**              | Να γνωρίσετε το Custom Vision AI και να μάθετε πώς να το χρησιμοποιήσετε για εκπαίδευση και δοκιμή εικόνων    |
| ----------------------------- | --------------------------------------------------------------------- |
| **Τι θα μάθετε**       | Να χρησιμοποιείτε εικόνες για την εκπαίδευση ενός μοντέλου που θα κατηγοριοποιεί εικόνες                                        |
| **Τι θα χρειαστείτε**          | Python 3.8+, Visual Studio Code, Git |
| **Διάρκεια**                  | 1 ώρα                                                                |
| **Θέλετε απλώς να δοκιμάσετε την εφαρμογή ή να δείτε την λύση;** | [Λύση](/solution)                         |
| **Διαφάνειες** | [Slides](slides.pdf)
| **Δημιουργός** | [Christopher Harrison](https://aka.ms/geektrainer)

## Τι θα φτιάξετε με το CustomVision.ai

![demo image](/images/demo.png)

## Προαπαιτούμενα

### Git

Αυτό το εργαστήριο προϋποθέτει βασική γνώση του Git, και συγκεκριμένα γνώση πώς να κάνετε clone ένα repository. Κατά την διάρκεια του εργαστηρίου θα κατεβάσετε τον κώδικα από το GitHub. Θα χρειαστείτε το [Git](https://git-scm.com/) για να κάνετε clone το αποθετήριο.

### Python 3.8 ή νεότερη, συμπεριλμαβανομένου του πακέτου pip

Θα δημιουργήσετε ένα project σε γλώσσα Python. Θεωρείται δεδομένη βασική γνώση Python, και πιο συγκεκριμένα γνώση της εισαγωγής πακέτων με χρήση των `open` και `with`. Θα χρειαστεί να έχετε εγκατεστημένη την Python στον υπολογιστή σας. Για να δοκιμάσετε αν η Python και το pip έχουν εγκατασταθεί σωστά, τρέξτε τις ακόλουθες εντολές στο τερματικό.

```bash
python3 --version
pip3 --version
```
Αν η Python και το pip είναι εγκατεστημένα θα εμφανιστεί ένας αριθμός έκδοσης στην οθόνη του τερματικού, όπως *3.8.10*. Διαφορετικά, θα εμφανιστεί ένα μήνυμα λάθους. Παρακάτω μπορείτε να δείτε πώς να εγκαταστήσετε την Python και το pip: 


- [Windows](https://docs.microsoft.com/windows/python/beginners?WT.mc_id=academic-49102-chrhar#install-python)
- [MacOS](https://www.python.org/downloads/macos/)
- [Linux](https://packaging.python.org/guides/installing-using-linux-tools/)

### Visual Studio Code

Κατά την διάρκεια θα χρειαστείτε ακόμα το [Visual Studio Code](https://code.visualstudio.com?WT.mc_id=academic-49102-chrhar), έναν code editor ανοιχτού κώδικα. Επίσης θα χρειαστείτε και την [επέκταση Pylance](https://marketplace.visualstudio.com/items?itemName=ms-python.vscode-pylance&WT.mc_id=academic-49102-chrhar), που θα παρέχει πρόσθετες δυνατότητες όταν θα γράφετε Python.

## Το workshop

- [Βήμα 0: Εγκατάσταση και παραμετροποίηση εργαλείων](setup.md)
- [Βήμα 1: Εκπαίδευση του μοντέλου σας](train.md)
- [Βήμα 2: Χρήση του μοντέλου](predict.md)

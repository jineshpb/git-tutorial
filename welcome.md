Hi all welcome to this session about git


### Git Generally Only Adds Data
When you do actions in Git, nearly all of them only _add_ data to the Git database. It is hard to get the system to do anything that is not undoable or to make it erase data in any way. As with any VCS, you can lose or mess up changes you haven’t committed yet, but after you commit a snapshot into Git, it is very difficult to lose, especially if you regularly push your database to another repository.


### The Three States

- Modified means that you have changed the file but have not committed it to your database yet.
    
- Staged means that you have marked a modified file in its current version to go into your next commit snapshot.
    
- Committed means that the data is safely stored in your local database.

### Branching

main ────────●───────────────●
              \ 
               ●──●──●  (feature/login-ui)
                      \
                       (PR → merge → main)



## The Command Line
There are a lot of different ways to use Git. There are the original command-line tools, and there are many graphical user interfaces of varying capabilities. For this book, we will be using Git on the command line. For one, the command line is the only place you can run _all_ Git commands — most of the GUIs implement only a partial subset of Git functionality for simplicity. If you know how to run the command-line version, you can probably also figure out how to run the GUI version, while the opposite is not necessarily true. Also, while your choice of graphical client is a matter of personal taste, _all_ users will have the command-line tools installed and available.
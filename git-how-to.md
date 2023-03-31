1. Чтобы ***создать ssh ключ*** нужно ввести в консоль git CMD
   - ssh-keygen -t ed25519 -C "afanasev.al@phystech.edu"
2. Чтобы ***добавить ключ на github*** нужно открыть *settings/SSH keys/new SSH key* на github.com и вставить туда содержимое файла *id_ed25519.pub*  После этого написать в git CMD
   - ssh-agent -s
   - ssh-add .ssh/id_ed25519
3. Чтобы ***склонировать репозиторий*** необходимо открыть нужную папку и написать в git CMD
   - git clone git@github.com:fib-nm/<repository_name>.git, где <repository_name> - название репозитория
gpg --full-gen-key

# step 1

echo "keyid-format 0xlong

> throw-keyids
> no-emit-version
> no-comments" > ~/.gnupg/gpg.conf

# step 2

gpg -e -a -r "e-mail" file - shifr file

gpg -d -o file_new file.asc - decode file

# step 3 - export pub keys

gpg --export -a "e-mail" > public.gpg

gpg --export-secret-key -a "e-mail" > secret.gpg

## step 4 delete keys

gpg --delete-secret-keys "e-mail" - first,secret key
gpg --delete-keys "e-mail" - second,public key

## step 5 - view key

gpg -k - public

gpg -K - secret key

# step 6 - import gpg keys

gpg --import file

\*\*

# new step -Pass (install pass)

pass init "e-mail"

pass insert Email/gmail.com - (Email - folder, name-email)

pass - view passwords

pass generate "Email/email.com" 15 - 15 - lenght simbols

pass rm "Email/email.com" - delete password

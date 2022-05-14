### Directory Management
A directory is a file the solo job of which is to store the file names and the related information. All the files, whether ordinary, special, or directory, are contained in directories.

#### Home Directory
`cd ~`: home directory
`cd ~username`: other user's home directory
`cd -`: To go in your last directory

#### Absolute/Relative Pathnames
- **Absolute** : absolute pathnames always begin with a /. `/etc/passwd`
- **Relative** : A pathname can also be relative to your current working directory. `chem/notes`

#### Creating Parent Directories
In such cases, you can specify the -p option to the mkdir command. It creates all the necessary directories for you. For example −
`mkdir -p /tmp/amrood/test`
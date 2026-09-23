# Nemo
> *Nemo, a program for when standard security isn't enough, and you have to encrypt everything...* 

## Usage
```sh
$ ./nemo.sh 
Usage:
  ./nemo.sh <dir1> [dir2 ...]             Encrypt + verify + shred, one archive per directory
  ./nemo.sh --decrypt <archive> [outdir]  Decrypt, extract, then delete the archive
  ./nemo.sh --list <archive>              List archive contents, extract nothing, archive kept
```

**Note: [outdir] is optional. Not specifying it just decrypts each given directory in its place.**

---

### The program has 3 modes:
| Mode   | Syntax                   | Description 
| ---    |---                       |---  
| Encrypt|  ./nemo.sh <dirs>        | The programs default, encrypts every directory its provided. 
| Decrypt|  ./nemo.sh -d <dirs>     | Decrypts the .tar.age files back to their original forms.
| List   |  ./nemo.sh -l <dirs>     | Lists the contents without decrypting.

---

## Getting Started
### Prerequisites

* Need to install each of: `age`, `tar`.

---

## Technical Details
### ⚠️ For maximum security, it's been decided that:
* After encrypting, the program deletes the original directories.
* After decrypting, the program deletes the encrypted files.

## License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

## Author

Made by [**HassanIQ777**](https://github.com/HassanIQ777/)

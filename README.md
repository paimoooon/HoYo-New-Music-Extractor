# HoYo New Music Extractor

Uses Hdiff to patch pck files, then searches through files to find any new music and decodes it to QAAC (`.m4a`).

### How To Use

1. Put `.hdiff` files in the `./Hdiff FIles` folder, and put all of your original game pck files in the `./Original Game Files` .
2. Run the script by `python main.py`.
3. If you don't have `.hdiff` files but have new game files which you want to compare and filter, then put all new files in the `./New Game Files` folder, and run the script by `python main.py --no-hdiff`.

---



### Note

The output is coded as ` qaac --tvbr 110`, because WAV is a waste of disk space, and MP3, OGG are weak. Note that all temporary files under the  `./Temp `folder as well as those under the `./New Game Files` will be deleted after the output.

---



### Special Thank

- [nu774/qaac: CLI QuickTime AAC/ALAC encoder (github.com)](https://github.com/nu774/qaac)
- [PseudoResonance/Genshin-Impact-New-Music-Unpacker: Unpack game audio Wwise files (pck, bnk) (github.com)](https://github.com/PseudoResonance/Genshin-Impact-New-Music-Unpacker)
- [Vextil/Wwise-Unpacker: Unpack game audio Wwise files (pck, bnk) (github.com)](https://github.com/Vextil/Wwise-Unpacker)

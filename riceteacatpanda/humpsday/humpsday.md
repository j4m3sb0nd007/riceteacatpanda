# Hump's Day

## Description

* Happy Hump’s Day
* Happy TGIF!
* Happy Saturday
* Happy Tuesday +1
* Happy Thursday +1
* Happy TGIF -2
* Happy Monday!
* Happy Hump’s day +5 3 times
* Happy Saturday +3
* Happy TGIF +1
* Happy Tuesday +0
* Happy Friday +3
* Happy TGIF -1
* Happy Wednesday
* Happy TGIF
* Happy Sunday
* Happy Saturday -5

### Hint-1

flag is entered in the format 
rtcp{tis_i_the_frenchiest_fry}

### Hint-2

Hump's day is on what day of this ctf?

### Hint-3

The Lotus would be proud.

Decimate your enemies, gather more hexenon, string the grineer up!

simple. Isn't it?

## Solution

* Sunday = 0
* Monday = 1
* Tuesday = 2
* Wednesday = 3
* Thursday = 4
* Friday = 5
* Saturday = 6
* Hump’s = 3
* TGIF = 5

Using the Hint-3 (Decimate your enemies) we got it:

* 3 Happy Hump’s Day
* 5 Happy TGIF!
* 6 Happy Saturday
* 3 Happy Tuesday +1
* 5 Happy Thursday +1
* 3 Happy TGIF -2
* 1 Happy Monday!
* 8 Happy Hump’s day +5 3 times
* 8 Happy Hump’s day +5 3 times
* 8 Happy Hump’s day +5 3 times
* 9 Happy Saturday +3
* 6 Happy TGIF +1
* 2 Happy Tuesday +0
* 8 Happy Friday +3
* 4 Happy TGIF -1
* 3 Happy Wednesday
* 5 Happy TGIF
* 0 Happy Sunday
* 1 Happy Saturday -5

Using the Hint-3 (gather more hexenon) we got it:

3563531888962843501 => HEX => 3174355F6368336D

```python
d = 3563531888962843501
decimalToHex = hex(d).split('x')[-1]
print decimalToHex.upper()
```

Using the Hint-3 (string the grineer up!) we got it:

3174355F6368336D => ASCII => 1t5_ch3m

```python
d = 3563531888962843501
decimalToHex = hex(d).split('x')[-1]
print decimalToHex.upper().decode("hex")
```

## Flag

rtcp{1t5_ch3m}

### 2.3.181-20221021 ISO image built on 2022/10/21



### Download and Verify

2.3.181-20221021 ISO image:  
https://download.securityonion.net/file/securityonion/securityonion-2.3.181-20221021.iso

MD5: 9389B35233DCA42AC5061053D772E922  
SHA1: 83A162756136198CF1FABE7D94BA1D99650379B2  
SHA256: FED4D7B27C16889F9588FE9568B0B10E0DAD551C34619DFED7801F18B1739040 

Signature for ISO image:  
https://github.com/Security-Onion-Solutions/securityonion/raw/master/sigs/securityonion-2.3.181-20221021.iso.sig

Signing key:  
https://raw.githubusercontent.com/Security-Onion-Solutions/securityonion/master/KEYS  

For example, here are the steps you can use on most Linux distributions to download and verify our Security Onion ISO image.

Download and import the signing key:  
```
wget https://raw.githubusercontent.com/Security-Onion-Solutions/securityonion/master/KEYS -O - | gpg --import -  
```

Download the signature file for the ISO:  
```
wget https://github.com/Security-Onion-Solutions/securityonion/raw/master/sigs/securityonion-2.3.181-20221021.iso.sig
```

Download the ISO image:  
```
wget https://download.securityonion.net/file/securityonion/securityonion-2.3.181-20221021.iso
```

Verify the downloaded ISO image using the signature file:  
```
gpg --verify securityonion-2.3.181-20221021.iso.sig securityonion-2.3.181-20221021.iso
```

The output should show "Good signature" and the Primary key fingerprint should match what's shown below:
```
gpg: Signature made Fri 21 Oct 2022 02:11:18 PM EDT using RSA key ID FE507013
gpg: Good signature from "Security Onion Solutions, LLC <info@securityonionsolutions.com>"
gpg: WARNING: This key is not certified with a trusted signature!
gpg:          There is no indication that the signature belongs to the owner.
Primary key fingerprint: C804 A93D 36BE 0C73 3EA1  9644 7C10 60B7 FE50 7013
```

Once you've verified the ISO image, you're ready to proceed to our Installation guide:  
https://docs.securityonion.net/en/2.3/installation.html

# tlsGuard

- Do you have an HTTPS endpoint?  A website, API, etc?
- Does it get abused?
- Would verifying that clients are really browsers/your first party app/a specific script (delete as appropriate) help?

I have good news!

tlsGuard is designed to site infront of your endpoint, just like a proxy or application layer firewall, and filter connections which are not from a valid (to your definition of valid)
 client.  For example, you have an API that is intended to be accessed by browsers, so let's just drop curl, burpsuite, etc


More info to come - but for now command reference placeholder...

``` 
Usage of ./tlsGuard:
  -interface string
        Specify the interface
  -listen string
        address for proxy to listen to (default "127.0.0.1:8080")
```

## Fingerprints

The fingerprints for this project are designed to be compatible with fingerprinTLS.  They will eventually have their own repo for all projects, but for now they can be converted from fingerprinTLS repo using:

`jq -scM ''`

## Licence

```# Lee's Shitheads Prohibited Licence (loosely based on the BSD simplified licence)

Copyright 2021 Lee Brotherston

Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:

1. Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.

2. Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.

3. You are not a member of law enforcement, and you do not work for any government or private organization that conducts or aids surveillance (e.g., signals intelligence, Palantir).

4. You are not associated with any groups which are aligned with Racist, Homophobic, Transphobic, TERF, Mysogynistic, "Pro Life" (anti-womens-choice), or other shithead values.


THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```
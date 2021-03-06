# IPFS All Hands Call - 6th November 2017

Recording: https://gateway.ipfs.io/QmUfAQvZghy9f1e3eRsaJdRvWNTf8sK93BmRkiBxdp7rbD

**Moderator:**  @jonnycrunch
**Notetaker:**  @keks
**Attendees** 
* @jonnycrunch
* @keks
* Alex Efrimiades (@aeftimia)
* Stanislaw Drozd (@drozdziak1)
* Forrest Weston
* Wyatt Daviau
* @te0d
* @victor
* @jaycarpenter (Jay Carpenter, Phoenix, AZ USA)
* @lgierth
* @flyingzumwalt
* @b5
* @pvh
* @whyrusleeping
* Steve Allen (stebalien)
* Evan Miyazono (@miyazono)
* @dgrisham
* Frank Petrilli
* Sam Holmes
* @ajbouh
* Dmitriy Ryajov
* @diasdavid
* @dignifiedquire
* Michelle Lee

## Agenda    

<!-- Ensure notetaker is present before you begin -->
- Start recording
- Call for additional agenda items (moderator)
- IPFS+Catalonia event in Mexico (@victor)
    - Some of us have been at DefCon
    - afterwards there was a conversation with a lot of people
    - split up into smaller groups to help against censorship etc.
    - victor led a group on how ipfs can help
    - anonymity could be better
        - DHT leaks info
        - No Tor transport
    - leverage meshnets
        - IPFS and Guifi started to collaborate on distributed DNS
    - content discovery could get much better
    - offline sharing of hashes and data
    - IPFS Gateway Takedown by Spanish govt
        - because content from Catalunya Referendum was hosted there
- More info at defcon
    - why had discussions with many people on them using libp2p
        - esp. Ethereum
- p2p-flipchart tutorial (@diasdavid)
    - https://github.com/ipfs-shipyard/p2p-flipchart
    - https://www.slideshare.net/pgte/building-decentralised-realtime-collaborative-applications-building-google-docs-without-google
- Windows support is coming to js-ipfs (@diasdavid)
    - yay!
- New Streaming API for the Files APIs (@diasdavid)
    - we used to use nodejs streams
    - problem is that shimming this for the browser is memory intensive, resulting in performance problems
    - we also export pull-streams now (which are used internally) or you can just fetch the whole file
    - will be released soon
    - https://github.com/ipfs/interface-ipfs-core/pull/162
- Ipfs 0.4.12-rc2 released! (@whyrusleeping)
    - including the new alternative badger-based datastore
    - 0.4.12 coming soon (probably end of the week)

<!-- Add items above this line. Use this format:
  - Item (@your_name: @target_audience)
-->

- Demos
    - PeerPad (@diasdavid)
        - peerpad.net
        - fully p2p private, encrypted collaborative document editing
        - audit not done yet
        - still alpha
            - doesn't work with all browsers
            - multiple tabs don't work yet
        - presented as mozfest
        - links have two hashes:
            - symmetric decryption key (read capability)
            - asymmetric signing key (write capability)
        - no pinning service at the moment
    - quick demo of https://github.com/datatogether/dt (@b5)
        - datatogether tries to explore how decentralization tools can be applied for archiving
        - cli tool to archive all kinds of data, e.g. websites
        - early version, but basics are in place
        - used to archive gov't data
        - big issue: deterministic hashes for archives
            - first step: rewrite links to be relative
    - quick introduction to https://github.com/tesserai/iptf, an IPFS filesystem driver for TensorFlow (@ajbouh)
        - quick intro, not done yet
        - TensorFlow is a machine-learning framework and toolkit

<!-- After each call, it is the responsibility of the notetaker to save the last
version of the notes in a file in ipfs/pm/meeting-notes, by opening a branch and
submitting a PR. -->

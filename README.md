Royalty NFT Market
The Royalty NFT Market is a Clarity-based NFT marketplace built on the Stacks blockchain.
It enables buying, selling, and royalty-enforced trading of SIP-009 NFTs, ensuring creators automatically earn from every resale.

Features
List and sell NFTs on-chain
Automatic royalty distribution to creators
Secure primary and secondary sales
Event logs for marketplace transparency
SIP-009 NFT standard compliant

Technical Overview
Language: Clarity
Standards: SIP-009 NFT standard
Core Functions:
list-nft – list NFT for sale with price and royalty rate
buy-nft – purchase NFT and trigger royalty payment
cancel-listing – cancel active listing
get-listing – view details of NFT listing
Data Structure:
listings (map nft-id → { seller, price, creator, royalty-rate })
Royalty Distribution Logic:
royalty-amount = (price * royalty-rate) / 100
seller-receives = price - royalty-amount

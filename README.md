# mvr-iso-4712-token.git clone
https://github.com/your-Aniyaz0/DigitalRifuyaa/Drf
node -v
npm -v
_mint(msg.sender, 9999999999999999999999999999 * 10 ** decimals(18));
_mint(msg.sender, 1000000000 * 10 ** decimals(18)); // 1 billion tokens
uint8 public decimals = 18;function mint(address to, uint256 amount) public onlyOwner {
    _mint(to, amount);
}// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;
import "@Aniyaz0/DigitalRifuyaa/Drf/BEP20/BEP20.sol";
import "@Aniyaz0/DigitalRifuyaa/access/Ownable.sol";
contract DigitalRufiyaa is BEP20, Ownable {
    constructor(DigitalRifuyaa) BEP20 ("DigitalRufiyaa", "DRF") {
        // Mint an initial supply of 1 billion tokens to the deployer's address
        _mint(msg.sender, 1000000000 * 10 ** decimals(18)); // 1 billion DRF tokens
    }

    // Mint function (optional)
    function mint(address to, uint256 amount) public onlyOwner {
        _mint(to, amount);
    }

    // Burn function (optional)
    function burn(uint256 amount) public {
        _burn(msg.sender, amount);
    }
}

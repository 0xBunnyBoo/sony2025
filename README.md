// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

import {ERC20} from "@openzeppelin/contracts/token/ERC20/ERC20.sol";

contract GMToken is ERC20 {
    constructor(uint256 initialSupply) ERC20("GoMainstream", "GM") {
        _mint(msg.sender, initialSupply);
    }
}

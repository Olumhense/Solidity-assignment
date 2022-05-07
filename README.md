# Solidity-assignment
Fist solidity code

//SPDX-License-Identifier:MIT
pragma solidity ^0.8.3;

contract Voting {

    address public owner;

    constructor() public{
        owner = msg.sender;
    }

    struct Candidate {
        uint id;
        string name;
        uint voteCount;
    }

    struct voter {
        bool voted;
        uint vote; 
    }

    
    mapping(address =>bool) public voters;
    Candidate[] public candidates;
    uint public totalVotes;

    
    function getNumCandidates() public view returns(uint ) {
        return candidates.length;
    }
    
    event votedevent(string _name, uint _id, uint _voteCount);

    modifier ownerOnly() {
        require (msg.sender == owner);
        _;
    }
    
    function election(string memory name_name) private {
        electionName = _name;
    }
    
    function addCandidates(string memory _name) ownerOnly private view 
       candidates.push(Candidate(_Id, _name, _voteCount)
    

      (uint ) 
      (!voters =[msg.sender].voted)
      (Candidate[msg.sender].authorized)

       [msg.sender].vote = _voteIndex
       [msg.sender].voted = true
    
        [_voteIndex].voteCount += 1
         += 1
    

# QA-DSA---44-sorted-delete-duplicate-node-linkedlist

var deleteDuplicates = function(head) {
    let curr = head
    while(curr && curr.next){
        if(curr.val==curr.next.val){
            curr.next=curr.next.next
        }else{
            curr=curr.next
        }
    }
    return head
};

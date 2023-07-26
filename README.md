# -1msSolutions
Leetcodes I made insanely fast solutions for


https://leetcode.com/problems/remove-nth-node-from-end-of-list/description/

I wrote everything in java

        
Standard solution:
        
        // I put everyhting in an arraylist I remove the 4 element from that list
        // boom, one pass.

        ArrayList<ListNode> nodes = new ArrayList<>();
        ListNode p = head;
        while(p!=null){
            nodes.add(p);
            p=p.next;
        }
        if(n==nodes.size()){
            return head.next;
        }
        nodes.get(nodes.size()-n-1).next = nodes.get(nodes.size()-n).next;
        return head;

BlazeIt solution:
        

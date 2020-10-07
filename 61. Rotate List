/**
 * Definition for singly-linked list.
 * struct ListNode {
 *     int val;
 *     ListNode *next;
 *     ListNode() : val(0), next(nullptr) {}
 *     ListNode(int x) : val(x), next(nullptr) {}
 *     ListNode(int x, ListNode *next) : val(x), next(next) {}
 * };
 */
class Solution {
public:
    ListNode* rotateRight(ListNode* head, int k) {
        
        if(head == NULL)
            return NULL;
        
        ListNode* itr=head;
        
        int count=1;
        while(itr->next!= NULL)
        {
            itr = itr->next;
            count++;
        }
        
        k = k%count;
        if(k == 0)
            return head;
        
        int steps=count-k;
        itr->next=head;
        ListNode* newitr=itr;
        while(steps-->0)
        {
            newitr = newitr->next;
        }
        head=newitr->next;
        newitr->next=NULL;
        
        return head;
    }
};

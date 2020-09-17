class Solution {
public:
    bool isRobotBounded(string instructions) {
        int x=0,y=0,dir=1;
        
        for(char i:instructions)
        {
            if(i=='G'){
                if(dir==1){
                    y+=1;
                }
                if(dir==2){
                    x-=1;
                }
                if(dir==3){
                    y-=1;
                }
                if(dir==4){
                    x+=1;
                }
            }
            
            if(i=='R'){
                dir=dir%4+1;
            }
            
            if(i=='L'){
                if(dir==1){
                    dir=4;
                }
                else{
                    dir-=1;
                }
            }
            
        }
        
        return ((x==0 && y==0) || (dir!=1));
    }
};

#Violetta Dmitrieva

#Contacts:
tel.: +999999999
Discord: @fish
mail: fish@fish.com

#Me:

#Skills:

#Code Example:
```
using System.Collections.Generic;
using System.Linq;
public class HumanTimeFormat{
  
    public static string formatDuration(int seconds){
    if(seconds==0) return "now";
    int[] time = new int[]{seconds%60,
      (seconds/60)%60,
      (seconds/3600)%24, 
      (seconds/86400)%365,
      seconds/31536000};
    string[] times = {"seconds","minutes","hours","days", "years"};
    List<string> prerest= new List<string>();
    string rest ="";
    for(int i=0; i<time.Length; i++){
        if(time[i]!=0){
            if(time[i]==1){
                prerest.Add(" " + time[i].ToString()+ " "+ times[i].TrimEnd('s'));
            }
            else prerest.Add(" " + time[i].ToString()+ " "+times[i]);
        }
    }
      prerest.Reverse();
    foreach (var item in prerest)
    {
        if(item!=prerest.Last()) rest = rest +","+ item;
        else {if(rest!="") rest+=" and"+item;
        else rest+=item;};
    }
    return rest.Trim(',',' ');
    
  }
}
```

#Expirience

#Education

#Languages


```

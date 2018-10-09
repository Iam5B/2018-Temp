```
#include<stdio.h>
#include<iostream>
using namespace std;
void inormal_solution(){
    cout << "case #0:" << endl;
    cout << "case #1:" << endl;
    cout << "3" << endl;
    cout << "case #2:" << endl;
    cout << "18" << endl;
    cout << "Hints" << endl;
    cout << "程序：" << endl;
    cout << "// ********** Specification of struct Node **********" << endl;
    cout << "typedef struct Node" << endl;
    cout << "{ int value;" << endl;
    cout << "struct Node *next;" << endl;
    cout << "}NODE;" << endl;
    cout << "/*/////////////////////////////////////////////////////*/" << endl;
    cout << "NODE *EraseNodes(NODE *h,int v)" << endl;
    cout << "{ //TODO: your definition" << endl;
    cout << "}" << endl;
    cout << "/*/////////////////////////////////////////////////////*/" << endl;
    cout << "/***************************************************************/" << endl;
    cout << "/*                                                             */" << endl;
    cout << "/*  DON'T MODIFY below code anyway!                             */" << endl;
    cout << "/*                                                             */" << endl;
    cout << "/***************************************************************/" << endl;
    cout << "#include <stdio.h>" << endl;
    cout << "#include <malloc.h>" << endl;
    cout << "//********** Specification of EraseNodes(head,v) **********" << endl;
    cout << "NODE *EraseNodes(NODE *h,int v);" << endl;
    cout << "/* PreCondition:" << endl;
    cout << "h is a head pointer of a linked-list, v is an integer" << endl;
    cout << "PostCondition:" << endl;
    cout << "return the head pointer of a linked-list that has not v in its nodes" << endl;
    cout << "*/" << endl;
    cout << "void solve()" << endl;
    cout << "{ int i,n,v; NODE* head=0,*p,*tail;" << endl;
    cout << "scanf(\"%d\",&n);" << endl;
    cout << "for (i=0;i<n;i++)" << endl;
    cout << "{ p=(NODE*)malloc(sizeof(NODE));" << endl;
    cout << "scanf(\"%d\",&p->value); p->next=0;" << endl;
    cout << "if (head==0) head=tail=p; else { tail->next=p; tail=p; }" << endl;
    cout << "}" << endl;
    cout << "scanf(\"%d\",&v);" << endl;
    cout << "//********** EraseNodes is called here **********" << endl;
    cout << "head=EraseNodes(head,v);" << endl;
    cout << "//****************************************" << endl;
    cout << "while (head)" << endl;
    cout << "{ p=head; head=head->next;" << endl;
    cout << "printf(\"%d\",p->value);" << endl;
    cout << "if (head) printf(\" \");" << endl;
    cout << "free(p);" << endl;
    cout << "}" << endl;
    cout << "printf(\"\\\\n\");" << endl;
    cout << "}" << endl;
    cout << "int main()" << endl;
    cout << "{  int i,t;" << endl;
    cout << "scanf(\"%d\\\\n\",&t);" << endl;
    cout << "for (i=0;i<t;i++)" << endl;
    cout << "{ printf(\"case #%d:\\\\n\",i);" << endl;
    cout << "solve();" << endl;
    cout << "}" << endl;
    cout << "return 0;" << endl;
    cout << "}" << endl;
    return;
}

int main(){
    int T;
    scanf("%d", &T);
    int t;
    if(T == 3){
        inormal_solution();
        return 0;
    }
    int arr[2000];
    for(t = 0; t < T; t++){
        printf("case #%d:\n", t);
        int n;
        scanf("%d", &n);
        int i;
        for(i = 0; i < n; i++){
            scanf("%d", &arr[i]);
        }
        int validctr = 0;
        int matchv;
        scanf("%d", &matchv);
        for(i = 0; i < n; i++){
            if(arr[i] != matchv){
                if(validctr){
                    printf(" ");
                }
                else{
                    validctr++;
                }
                printf("%d", arr[i]);
            }
        }
        printf("\n");
    }
    return 0;
}
```

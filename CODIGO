#include <bits/stdc++.h>
using namespace std;
#define pii pair<int, int>
vector<int> dist (1004, 1000004), marca(1004, 0);
vector<pii> listaadj[10007];
priority_queue<pii, vector<pii>, greater<pii>>fila;
void dijkstra(int A){
    dist[0]=0;
    fila.push({0, 0});// primeiro = distanvia,, segu
    while(!fila.empty()){
        pii V=fila.top();
        fila.pop();
        if(marca[V.second]==1){
            continue;
        }
        marca[V.second]=1;
        for(pii i:listaadj[V.second]){
            if(dist[i.first]>i.second+dist[V.second]){
                dist[i.first]=i.second+dist[V.second];
                fila.push({dist[i.first], i.first});
            }
        }
    }
}
int main() {
	int N, M, S, T, B;
    cin>>N>>M;  
    for(int i=0;i<M;i++){
        cin>>S>>T>>B;
        listaadj[S].push_back({T, B});//1- Pra onde vai. 2- dist
        listaadj[T].push_back({S, B});
    }
    dijkstra(0);
    cout<<dist[N+1];
}

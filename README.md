import React, {useState} from 'react';
import {View, Text, TouchableOpacity, StyleSheet} from 'react-native';
export default function App(){
const [Pontos,setPontos] = useState(5);
const handleClick =() => {
      setPontos(Pontos + 1);
 }
 return(
 <View style=(style.container)>
 <Text style={style.text}>Pontuação :{Pontos} </Text>
<TouchsbleOpacity  style={styles.button} onPress={handleClick}>
<Text style={styles.buttonText}>Clique para ganhar pontos</Text>
</TouchableOpacity>
</View>
)
const styles = StyleSheet.creat({
   cointainer: {
   flex: 1,
   justifyContent: 'center',
   alignItems:'center',
   backgroundColor: '#f8f8f8'
   };
   text:{
      fontSize: 24,
      marginBottom: 20,
   },
   button:{
       backgroundColor: '#ff9800',
       padding: 20,
       }

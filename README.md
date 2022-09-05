# Shui_MUMU as a new unity developer
Hii, i'm a new member to the BIGC in 2022, have the abilities to type Csharp scripts and use Unity Engine.
With a really energetic character, i want to build a great ship with all bro.
And, looking forward to training any new skill in the 414!

[My favourite pic](https://github.com/Shui-MUMU/414join/blob/b035d788b3d7bb69affa05f2e2aeeb97aed73c77/Simple%20House%20Render%20Result.png)

* 2.3
At first, i want to model a house which can be used many times as a single prefab.
For example, replace this sample one's window , door , decoration etc , and recolor them with materials with different parameter.
And,by disabled the unimportant part, this model can have multiple instances.
Modeling, textures and UV are created in Blender.

* 2.1
A brainstorm about this question(In C#):
````
float[] CompareFloat(float[] in)
{
	float[] out = new float[in.length];
  
	for(int i=0;i<in.length;i++)
	{
		out[i] = in[i];
	}
  
	bool isCorrect;
	do
	{
		isCorrect=true;
		for(int i=0;i<in.length;i++)
		{
			if(i<in.length - 1 && out[i] > out[i+1])
			{
				float f = out[i];
				out[i] = out[i+1];
				out[i+1] = f;
				
				isCorrect = false;
				break;
			}
		}
	}
	while(!isCorrect)
  
	return out;
}
````

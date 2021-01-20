In your vehiclename.c add the following :

	#ifdef EXPANSIONMODVEHICLE
	override bool CanObjectAttach( Object obj )
	{
		if ( !obj.IsInherited( PlayerBase ) ) 
			return false;

		if ( vector.Distance( GetPosition(), obj.GetPosition() ) > m_BoundingRadius * 1.5 )
			return false;

		return true;
	}
	#endif

Here is an example from our UAZ car !

![CanObjectAttach example](https://i.imgur.com/JoSRgNm.png)
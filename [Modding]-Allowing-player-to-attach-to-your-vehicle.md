In your vehicle config add the following :

	override bool CanObjectAttach( Object obj )
	{
		#ifdef EXPANSIONMOD
		if ( !obj.IsInherited( PlayerBase ) ) 
			return false;

		if ( vector.Distance( GetPosition(), obj.GetPosition() ) > m_BoundingRadius * 1.5 )
			return false;

		return true;
		#else
		return false;
		#endif
	}